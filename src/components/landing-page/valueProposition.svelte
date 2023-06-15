<script lang="ts">
    import FaRegMoneyBillAlt from 'svelte-icons/fa/FaRegMoneyBillAlt.svelte'
    import DiDatabase from 'svelte-icons/di/DiDatabase.svelte'
    import FaHandshake from 'svelte-icons/fa/FaHandshake.svelte'
    import IoMdHammer from 'svelte-icons/io/IoMdHammer.svelte'
    const features = [
  {
    name: 'Customized Approach',
    description:
      'We understand that every client is different, which is why we take a personalized approach. We delve deep into their challenges, requirements, and goals, ensuring that our solutions are specifically tailored to address their pain points effectively.',
      Icon:IoMdHammer,
  },
  {
    name: 'Time and Cost Savings',
    description:
      'We recognize the importance of efficiency and cost-effectiveness. Through our expertise and streamlined processes, we help clients save valuable time and minimize unnecessary expenses, delivering optimal value for their investment.',
    Icon: FaRegMoneyBillAlt
  },
  {
    name: 'Scalability and Future-Proofing',
    description:
      'We build solutions that are scalable and future-proof, ensuring that our clients\' software infrastructure can easily adapt and grow alongside their business. Our goal is to provide technology solutions that can accommodate their evolving needs.',
      Icon:DiDatabase
  },
  {
    name: 'Collaborative Partnership',
    description:
      'We believe in establishing strong relationships with our clients. We work closely with them, fostering a collaborative partnership that ensures their goals are met. We value their input, actively involve them in the decision-making process, and prioritize their satisfaction throughout the engagement.',
      Icon: FaHandshake
  },
]

</script>


<div class="bg-[#111827] py-24 sm:py-32">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl lg:text-center">
        <h2 class="text-base font-semibold leading-7 text-indigo-600">OUR VALUE PROPOSITION</h2>
        <p class="mt-2 text-3xl font-bold tracking-tight text-white sm:text-4xl">Delivering exceptional results and providing customized solutions tailored to our clients' unique needs. </p>
      </div>
      <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-4xl">
        <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-10 lg:max-w-none lg:grid-cols-2 lg:gap-y-16">
            {#each features as {name,description,Icon}(name)} 

            <div class="relative pl-16">
              <dt class="text-base font-semibold leading-7 text-[#94A3B8]">
                <div class="absolute left-0 top-0 flex h-10 w-10 items-center justify-center rounded-lg text-white bg-indigo-600 p-1">
                  <Icon/>
                </div>
                {name}
                
              </dt>
              <dd class="mt-2 text-base leading-7 text-[#737373]">{description}</dd>
            </div>
            {/each}
        </dl>
      </div>
    </div>
  </div>