<script lang="ts">
    import MdDeveloperMode from 'svelte-icons/md/MdDeveloperMode.svelte'
    import FaRegHandshake from 'svelte-icons/fa/FaRegHandshake.svelte'
    import GoBeaker from 'svelte-icons/go/GoBeaker.svelte'
    import IoIosBriefcase from 'svelte-icons/io/IoIosBriefcase.svelte'
    import GiLifeSupport from 'svelte-icons/gi/GiLifeSupport.svelte'
    import FaNetworkWired from 'svelte-icons/fa/FaNetworkWired.svelte'
    let services = [
        {
            title:"Software Development",
            subTitle:"Our expert team excels in developing customized software solutions that cater to your specific requirements. We leverage the latest technologies and industry best practices to deliver efficient, scalable, and secure applications that drive your business forward. By partnering with us, you can benefit from enhanced productivity, streamlined processes, and a competitive advantage in the market.",
            Icon:MdDeveloperMode,
        },
        {
            title:"Technical Consulting",
            subTitle:"Our technical consulting services provide you with strategic guidance and expert advice to navigate the complex technology landscape. Whether you need assistance with software architecture, system integration, or technology selection, our consultants are here to help. By leveraging our expertise, you can make informed decisions, optimize your technology investments, and achieve your business objectives effectively.",
            Icon:FaRegHandshake,
        },

        {
            title:"Quality Assurance and Testing",
            subTitle:"We understand the importance of delivering reliable and high-performing software solutions. Our comprehensive quality assurance and testing services ensure that your applications meet the highest standards of functionality, performance, and security. By partnering with us, you can minimize risks, improve user satisfaction, and maintain the integrity of your software throughout its lifecycle.",
            Icon:GoBeaker
        },

        {
            title:"Project Management",
            subTitle:" Our experienced project managers will ensure the successful execution of your software projects from start to finish. We follow proven project management methodologies, enabling us to effectively plan, execute, and control projects to deliver on time and within budget. By entrusting your projects to us, you can enjoy seamless collaboration, clear communication, and efficient project delivery.",
            Icon:IoIosBriefcase
        },
        {
            title:"Maintenance and Support",
            subTitle:"Our commitment to your success extends beyond project completion. We provide ongoing maintenance and support services to ensure the optimal performance and longevity of your software applications. Our dedicated support team is available to address any issues, provide technical assistance, and implement updates or enhancements as needed.",
            Icon:GiLifeSupport,
        },
        {
            title:"Digital Transformation Solutions",
            subTitle:"Embrace the digital era with confidence. We offer comprehensive digital transformation solutions that help you modernize legacy systems, adopt cloud technologies, harness data analytics, and leverage emerging technologies to stay ahead of the curve.",
            Icon:FaNetworkWired
        }, 
        
    ]
</script>



<section class="text-gray-600 body-font ">
  <div class="container px-5 py-24 mx-auto">
    <div class="flex flex-wrap w-full mb-20 flex-col items-center text-center">
      <h1 class="sm:text-3xl text-2xl max-w-2xl font-bold leading-7 text-indigo-600 tracking-tight">Unlocking Your Potential: Our Comprehensive Consulting Services</h1>
      <p class="lg:w-1/2 max-w-xl w-full leading-relaxed text-gray-500 font-semibold">Partner with our consulting experts to unlock your company's full potential and achieve unparalleled success in a rapidly evolving digital landscape
      </p>
    </div>
    <div class="flex flex-wrap -m-4">
        {#each services as {title,subTitle,Icon}(title)}
            
        <div class="xl:w-1/3 md:w-1/2 p-4 ">
          <div class="border border-gray-200 p-6 rounded-lg min-h-[21rem]">
            <div class="w-10 h-10 inline-flex items-center justify-center rounded-full  text-indigo-500 mb-4">
              <Icon/>
            </div>
            <h2 class="text-lg font-semibold title-font mb-2 text-indigo-500">{title}</h2>
            <p class="leading-relaxed text-base">{subTitle}</p>
          </div>
        </div>
        {/each}
    
    </div>
    
  </div>
</section>
