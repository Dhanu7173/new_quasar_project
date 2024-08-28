<template>
<q-page class="flex min-h-full flex-col justify-center py-12 sm:px-6 lg:px-8">
  <div class="sm:mx-auto sm:w-full sm:max-w-md">
    <img class="mx-auto h-10 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="Your Company">
    <h2 class="mt-6 text-center text-2xl font-bold leading-9 tracking-tight text-gray-900">Sign in to your account</h2>
  </div>

  <div class="mt-10 sm:mx-auto sm:w-full sm:max-w-[480px]">
    <div class="bg-white px-6 py-12 shadow sm:rounded-lg sm:px-12">
      <div class="space-y-6" action="#" method="POST">
        <div>
          <label for="phone" class="block text-sm font-medium leading-6 text-gray-900">Phone</label>
          <div class="mt-2">
            <q-input
              outlined
              v-model="phone"
              label="Phone"
              dense
              class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-[#FFA500] sm:text-sm sm:leading-6"
            />
          </div>
        </div>

        <div>
          <label for="password" class="block text-sm font-medium leading-6 text-gray-900">Password</label>
          <div class="mt-2">
            <q-input
              outlined
              v-model="password"
              label="Password"
              dense
              class="block w-full rounded-md border-0 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-[#FFA500] sm:text-sm sm:leading-6"
            />
          </div>
        </div>

        <div class="flex items-center justify-between">
          <div class="flex items-center">
            <input id="remember-me" name="remember-me" type="checkbox" class="h-4 w-4 rounded border-gray-300 text-indigo-600 focus:ring-indigo-600">
            <label for="remember-me" class="ml-3 block text-sm leading-6 text-gray-900">Remember me</label>
          </div>

          <div class="text-sm leading-6">
            <a href="#" class="font-semibold text-indigo-600 hover:text-indigo-500">Forgot password?</a>
          </div>
        </div>

        <div>
          <button type="submit" class="flex w-full justify-center rounded-md bg-indigo-600 px-3 py-1.5 text-sm font-semibold leading-6 text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Sign in</button>
        </div>
      </div>

      <div>
        <div class="relative mt-10">
          <div class="absolute inset-0 flex items-center" aria-hidden="true">
            <div class="w-full border-t border-gray-200"></div>
          </div>
          <div class="relative flex justify-center text-sm font-medium leading-6">
            <span class="bg-white px-6 text-gray-900">Or continue with</span>
          </div>
        </div>

        <div class="mt-6 grid grid-cols-1 gap-4">
          <a href="#" class="flex w-full items-center justify-center gap-3 rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50 focus-visible:ring-transparent">
            <svg class="h-5 w-5" viewBox="0 0 24 24" aria-hidden="true">
              <path d="M12.0003 4.75C13.7703 4.75 15.3553 5.36002 16.6053 6.54998L20.0303 3.125C17.9502 1.19 15.2353 0 12.0003 0C7.31028 0 3.25527 2.69 1.28027 6.60998L5.27028 9.70498C6.21525 6.86002 8.87028 4.75 12.0003 4.75Z" fill="#EA4335" />
              <path d="M23.49 12.275C23.49 11.49 23.415 10.73 23.3 10H12V14.51H18.47C18.18 15.99 17.34 17.25 16.08 18.1L19.945 21.1C22.2 19.01 23.49 15.92 23.49 12.275Z" fill="#4285F4" />
              <path d="M5.26498 14.2949C5.02498 13.5699 4.88501 12.7999 4.88501 11.9999C4.88501 11.1999 5.01998 10.4299 5.26498 9.7049L1.275 6.60986C0.46 8.22986 0 10.0599 0 11.9999C0 13.9399 0.46 15.7699 1.28 17.3899L5.26498 14.2949Z" fill="#FBBC05" />
              <path d="M12.0004 24.0001C15.2404 24.0001 17.9654 22.935 19.9454 21.095L16.0804 18.095C15.0054 18.82 13.6204 19.245 12.0004 19.245C8.8704 19.245 6.21537 17.135 5.2654 14.29L1.27539 17.385C3.25539 21.31 7.3104 24.0001 12.0004 24.0001Z" fill="#34A853" />
            </svg>
            <span class="text-sm font-semibold leading-6">Google</span>
          </a>
        </div>
      </div>
    </div>

    <p class="mt-10 text-center text-sm text-gray-500">
      Not a member?
      <a href="#" class="font-semibold leading-6 text-indigo-600 hover:text-indigo-500">Start a 14 day free trial</a>
    </p>
  </div>
  <div
      class="h-screen w-screen flex items-end overflow-hidden absolute top-0 left-0 z-[-10] shrink-0"
    >
      <svg
        id="svg"
        viewBox="0 0 1440 390"
        xmlns="http://www.w3.org/2000/svg"
        class="transition duration-300 ease-in-out delay-150"
      >
        <defs>
          <linearGradient id="gradient" x1="0%" y1="80%" x2="100%" y2="50%">
            <stop offset="5%" stop-color="#FFA500"></stop>
            <stop offset="95%" stop-color="#EF820D"></stop>
          </linearGradient>
        </defs>
        <path
          d="M 0,400 L 0,300 C 137.3214285714286,323.94642857142856 274.6428571428572,347.89285714285717 388,328 C 501.3571428571428,308.10714285714283 590.7499999999998,244.375 703,204 C 815.2500000000002,163.625 950.3571428571429,146.60714285714283 1077,129 C 1203.642857142857,111.39285714285715 1321.8214285714284,93.19642857142858 1440,75 L 1440,400 L 0,400 Z"
          stroke="none"
          stroke-width="0"
          fill="url(#gradient)"
          fill-opacity="0.4"
          class="transition-all duration-300 ease-in-out delay-150 path-0"
        ></path>
        <defs>
          <linearGradient id="gradient" x1="0%" y1="50%" x2="100%" y2="50%">
            <stop offset="5%" stop-color="#eb144c"></stop>
            <stop offset="95%" stop-color="#9900ef"></stop>
          </linearGradient>
        </defs>
        <path
          d="M 0,400 L 0,400 C 95.67857142857142,397.5178571428571 191.35714285714283,395.0357142857143 328,390 C 464.64285714285717,384.9642857142857 642.2500000000001,377.375 774,352 C 905.7499999999999,326.625 991.6428571428571,283.4642857142857 1095,251 C 1198.357142857143,218.53571428571428 1319.1785714285716,196.76785714285714 1440,175 L 1440,400 L 0,400 Z"
          stroke="none"
          stroke-width="0"
          fill="url(#gradient)"
          fill-opacity="0.53"
          class="transition-all duration-300 ease-in-out delay-150 path-1"
        ></path>
        <defs>
          <linearGradient id="gradient" x1="0%" y1="50%" x2="100%" y2="50%">
            <stop offset="5%" stop-color="#eb144c"></stop>
            <stop offset="95%" stop-color="#9900ef"></stop>
          </linearGradient>
        </defs>
        <path
          d="M 0,400 L 0,500 C 151.85714285714286,498.44642857142856 303.7142857142857,496.89285714285717 405,481 C 506.2857142857143,465.10714285714283 557.0000000000001,434.87499999999994 659,413 C 760.9999999999999,391.12500000000006 914.2857142857142,377.6071428571429 1053,356 C 1191.7142857142858,334.3928571428571 1315.857142857143,304.69642857142856 1440,275 L 1440,400 L 0,400 Z"
          stroke="none"
          stroke-width="0"
          fill="url(#gradient)"
          fill-opacity="1"
          class="transition-all duration-300 ease-in-out delay-150 path-2"
        ></path>
      </svg>
    </div>
</q-page>
</template>


<style>
.path-0 {
  animation: pathAnim-0 4s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}
@keyframes pathAnim-0 {
  0% {
    d: path(
      "M 0,400 L 0,300 C 137.3214285714286,323.94642857142856 274.6428571428572,347.89285714285717 388,328 C 501.3571428571428,308.10714285714283 590.7499999999998,244.375 703,204 C 815.2500000000002,163.625 950.3571428571429,146.60714285714283 1077,129 C 1203.642857142857,111.39285714285715 1321.8214285714284,93.19642857142858 1440,75 L 1440,400 L 0,400 Z"
    );
  }
  25% {
    d: path(
      "M 0,400 L 0,300 C 77.21428571428572,306.2321428571429 154.42857142857144,312.4642857142857 301,302 C 447.57142857142856,291.5357142857143 663.5000000000001,264.375 783,243 C 902.4999999999999,221.62499999999997 925.5714285714287,206.03571428571428 1019,179 C 1112.4285714285713,151.96428571428572 1276.2142857142858,113.48214285714286 1440,75 L 1440,400 L 0,400 Z"
    );
  }
  50% {
    d: path(
      "M 0,400 L 0,300 C 91.57142857142858,304.0892857142857 183.14285714285717,308.17857142857144 296,299 C 408.85714285714283,289.82142857142856 542.9999999999999,267.375 679,243 C 815.0000000000001,218.625 952.8571428571429,192.32142857142858 1080,164 C 1207.142857142857,135.67857142857142 1323.5714285714284,105.33928571428571 1440,75 L 1440,400 L 0,400 Z"
    );
  }
  75% {
    d: path(
      "M 0,400 L 0,300 C 95,301.5892857142857 190,303.17857142857144 322,297 C 454,290.82142857142856 622.9999999999999,276.875 739,258 C 855.0000000000001,239.125 918,215.32142857142858 1026,184 C 1134,152.67857142857142 1287,113.83928571428571 1440,75 L 1440,400 L 0,400 Z"
    );
  }
  100% {
    d: path(
      "M 0,400 L 0,300 C 137.3214285714286,323.94642857142856 274.6428571428572,347.89285714285717 388,328 C 501.3571428571428,308.10714285714283 590.7499999999998,244.375 703,204 C 815.2500000000002,163.625 950.3571428571429,146.60714285714283 1077,129 C 1203.642857142857,111.39285714285715 1321.8214285714284,93.19642857142858 1440,75 L 1440,400 L 0,400 Z"
    );
  }
}
</style>

      <style>
.path-1 {
  animation: pathAnim-1 4s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}
@keyframes pathAnim-1 {
  0% {
    d: path(
      "M 0,400 L 0,400 C 95.67857142857142,397.5178571428571 191.35714285714283,395.0357142857143 328,390 C 464.64285714285717,384.9642857142857 642.2500000000001,377.375 774,352 C 905.7499999999999,326.625 991.6428571428571,283.4642857142857 1095,251 C 1198.357142857143,218.53571428571428 1319.1785714285716,196.76785714285714 1440,175 L 1440,400 L 0,400 Z"
    );
  }
  25% {
    d: path(
      "M 0,400 L 0,400 C 100.53571428571428,393.9107142857143 201.07142857142856,387.82142857142856 334,381 C 466.92857142857144,374.17857142857144 632.2499999999999,366.625 761,350 C 889.7500000000001,333.375 981.9285714285713,307.67857142857144 1089,277 C 1196.0714285714287,246.32142857142858 1318.0357142857142,210.66071428571428 1440,175 L 1440,400 L 0,400 Z"
    );
  }
  50% {
    d: path(
      "M 0,400 L 0,400 C 129.25,404.80357142857144 258.5,409.60714285714283 399,396 C 539.5,382.39285714285717 691.25,350.375 785,324 C 878.75,297.625 914.5,276.89285714285717 1014,253 C 1113.5,229.10714285714283 1276.75,202.05357142857142 1440,175 L 1440,400 L 0,400 Z"
    );
  }
  75% {
    d: path(
      "M 0,400 L 0,400 C 94.17857142857142,393.30357142857144 188.35714285714283,386.60714285714283 317,366 C 445.64285714285717,345.39285714285717 608.7500000000001,310.875 731,292 C 853.2499999999999,273.125 934.6428571428571,269.8928571428571 1046,253 C 1157.357142857143,236.10714285714286 1298.6785714285716,205.55357142857144 1440,175 L 1440,400 L 0,400 Z"
    );
  }
  100% {
    d: path(
      "M 0,400 L 0,400 C 95.67857142857142,397.5178571428571 191.35714285714283,395.0357142857143 328,390 C 464.64285714285717,384.9642857142857 642.2500000000001,377.375 774,352 C 905.7499999999999,326.625 991.6428571428571,283.4642857142857 1095,251 C 1198.357142857143,218.53571428571428 1319.1785714285716,196.76785714285714 1440,175 L 1440,400 L 0,400 Z"
    );
  }
}
</style>

      <style>
.path-2 {
  animation: pathAnim-2 4s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}
@keyframes pathAnim-2 {
  0% {
    d: path(
      "M 0,400 L 0,500 C 151.85714285714286,498.44642857142856 303.7142857142857,496.89285714285717 405,481 C 506.2857142857143,465.10714285714283 557.0000000000001,434.87499999999994 659,413 C 760.9999999999999,391.12500000000006 914.2857142857142,377.6071428571429 1053,356 C 1191.7142857142858,334.3928571428571 1315.857142857143,304.69642857142856 1440,275 L 1440,400 L 0,400 Z"
    );
  }
  25% {
    d: path(
      "M 0,400 L 0,500 C 134.03571428571428,507.375 268.07142857142856,514.75 376,501 C 483.92857142857144,487.25 565.75,452.375 671,420 C 776.25,387.625 904.9285714285716,357.75 1037,334 C 1169.0714285714284,310.25 1304.5357142857142,292.625 1440,275 L 1440,400 L 0,400 Z"
    );
  }
  50% {
    d: path(
      "M 0,400 L 0,500 C 87.03571428571428,509.7678571428571 174.07142857142856,519.5357142857142 319,512 C 463.92857142857144,504.4642857142857 666.7500000000001,479.62500000000006 783,448 C 899.2499999999999,416.37499999999994 928.9285714285713,377.9642857142857 1024,348 C 1119.0714285714287,318.0357142857143 1279.5357142857142,296.5178571428571 1440,275 L 1440,400 L 0,400 Z"
    );
  }
  75% {
    d: path(
      "M 0,400 L 0,500 C 96.28571428571428,513.9821428571429 192.57142857142856,527.9642857142858 318,513 C 443.42857142857144,498.0357142857143 598.0000000000001,454.125 739,420 C 879.9999999999999,385.875 1007.4285714285716,361.5357142857143 1122,339 C 1236.5714285714284,316.4642857142857 1338.2857142857142,295.7321428571429 1440,275 L 1440,400 L 0,400 Z"
    );
  }
  100% {
    d: path(
      "M 0,400 L 0,500 C 151.85714285714286,498.44642857142856 303.7142857142857,496.89285714285717 405,481 C 506.2857142857143,465.10714285714283 557.0000000000001,434.87499999999994 659,413 C 760.9999999999999,391.12500000000006 914.2857142857142,377.6071428571429 1053,356 C 1191.7142857142858,334.3928571428571 1315.857142857143,304.69642857142856 1440,275 L 1440,400 L 0,400 Z"
    );
  }
}
</style>