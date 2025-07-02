<template>
  <div class="bg-gray-900 py-24 sm:py-32">
    <div class="mx-auto max-w-4xl px-6 lg:px-8 text-center">
      <div class="mb-2 text-blue-600 font-semibold text-sm tracking-widest">OUR VISION</div>
      <h2 class="text-4xl sm:text-5xl font-extrabold text-gray-900 mb-2">Your AI Journey, Our Long-Term Partnership</h2>
      <p class="text-lg text-gray-600 mb-10">Shaping the future of enterprise IT together</p>
    </div>
    <div class="mx-auto max-w-5xl px-2 lg:px-0">
      <div class="bg-white rounded-xl shadow p-8 flex flex-col md:flex-row gap-8 items-stretch">
        <div class="flex-1 text-left flex flex-col justify-between">
          <div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2">Beyond SaaS Replacement</h3>
            <p class="text-gray-700 mb-4">Saasinator aims to become the leading AI systems integrator and SaaS replacement services firm globally – known for building high-impact, bespoke AI apps that are <span class='text-blue-600 font-bold'>10x faster, smarter, and cheaper</span> than conventional software.</p>
            <p class="text-gray-700 mb-6">Over the next 5-10 years, we will evolve into a hybrid of services and IP-led app portfolio, building reusable frameworks and potentially low-code interfaces for faster, smarter, and cheaper AI solutions, ensuring your continuous innovation.</p>
          </div>
          <a href="#" class="inline-block rounded-md bg-blue-600 px-6 py-3 text-base font-semibold text-white shadow hover:bg-blue-700">Join Us on This Journey</a>
        </div>
        <div class="flex-1 flex flex-col items-center justify-center">
          <div class="w-full bg-blue-50 rounded-xl p-8 flex flex-col items-center">
            <div class="bg-blue-600 rounded-full p-3 mb-4">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="white" class="w-10 h-10"><path stroke-linecap="round" stroke-linejoin="round" d="M12 6v6l4 2" /></svg>
            </div>
            <h4 class="text-xl font-bold text-gray-900 mb-2">AI Transformation Roadmap</h4>
            <p class="text-gray-700 text-center mb-6">Our vision extends beyond immediate cost savings to continuous innovation and strategic advantage through AI.</p>
            <div class="w-full h-32 bg-gradient-to-r from-blue-500 to-blue-300 rounded-lg flex items-center justify-center">
              <span class="text-white font-semibold">AI Transformation Roadmap Diagram</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ArrowPathIcon, CloudArrowUpIcon, LockClosedIcon } from '@heroicons/vue/20/solid'

const features = [
  {
    name: 'Push to deploy',
    description:
      'Commodo nec sagittis tortor mauris sed. Turpis tortor quis scelerisque diam id accumsan nullam tempus. Pulvinar etiam lacus volutpat eu.',
    href: '#',
    icon: CloudArrowUpIcon,
  },
  {
    name: 'SSL certificates',
    description:
      'Pellentesque enim a commodo malesuada turpis eleifend risus. Facilisis donec placerat sapien consequat tempor fermentum nibh.',
    href: '#',
    icon: LockClosedIcon,
  },
  {
    name: 'Simple queues',
    description:
      'Pellentesque sit elit congue ante nec amet. Dolor aenean curabitur viverra suspendisse iaculis eget. Nec mollis placerat ultricies euismod.',
    href: '#',
    icon: ArrowPathIcon,
  },
]
</script>