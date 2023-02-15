<template>
  <div
    class="lg:first-of-type:hidden lg:last-of-type:hidden lg:after:content-[' '] lg:after:border-l lg:after:border-l-gray-600 lg:after:absolute lg:after:left-0 lg:after:top-[calc(50% + 25px)] lg:after:h-[calc(50% - 25px)] lg:mt-0 flex mt-8 lg:pt-1.5 lg:pr-0 lg:pb-4 lg:pl-20 lg:before:content-[' '] lg:before:border-l lg:before:border-l-gray-600 lg:before:absolute lg:before:left-0 lg:before:bottom-[calc(50% + 25px)] lg:before:h-[calc(50% - 25px)]"
  >
    <i
      class="place-items-center dark:text-gray-600 flex content-center w-8 h-8 text-gray-800 lg:top-[calc(50% - 25px)] lg:-left-6 lg:absolute lg:border-r lg:border-gray-600 lg:rounder-lg lg:w-12 lg:h-12"
    >
      <slot name="icon"></slot>
    </i>
    <div class="flex-1 ml-4">
      <h3 class="text-xl font-medium mb-1.5 text-800 dark:text-400">
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>
