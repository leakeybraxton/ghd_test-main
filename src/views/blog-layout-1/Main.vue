<template>
  <div class="intro-y flex flex-col sm:flex-row items-center mt-8">
    <h2 class="text-lg font-medium mr-auto">Blog Layout</h2>
    <div class="w-full sm:w-auto flex mt-4 sm:mt-0">
      <button class="btn btn-primary shadow-md mr-2">Add New Post</button>
      <Dropdown class="ml-auto sm:ml-0">
        <DropdownToggle class="btn px-2 box">
          <span class="w-5 h-5 flex items-center justify-center">
            <PlusIcon class="w-4 h-4" />
          </span>
        </DropdownToggle>
        <DropdownMenu class="w-40">
          <DropdownContent>
            <DropdownItem>
              <Share2Icon class="w-4 h-4 mr-2" /> Share Post
            </DropdownItem>
            <DropdownItem>
              <DownloadIcon class="w-4 h-4 mr-2" /> Download Post
            </DropdownItem>
          </DropdownContent>
        </DropdownMenu>
      </Dropdown>
    </div>
  </div>
  <div class="intro-y grid grid-cols-12 gap-6 mt-5">
    <!-- BEGIN: Blog Layout -->
    <div
      v-for="(faker, fakerKey) in $_.take($f(), 9)"
      :key="fakerKey"
      class="intro-y col-span-12 md:col-span-6 xl:col-span-4 box"
    >
      <div
        class="flex items-center border-b border-slate-200/60 dark:border-darkmode-400 px-5 py-4"
      >
        <div class="w-10 h-10 flex-none image-fit">
          <img
            alt="Icewall Tailwind HTML Admin Template"
            class="rounded-full"
            :src="faker.photos[0]"
          />
        </div>
        <div class="ml-3 mr-auto">
          <a href="" class="font-medium">{{ faker.users[0].name }}</a>
          <div class="flex text-slate-500 truncate text-xs mt-0.5">
            <a class="text-primary inline-block truncate" href="">{{
              faker.products[0].category
            }}</a>
            <span class="mx-1">•</span> {{ faker.formattedTimes[0] }}
          </div>
        </div>
        <Dropdown class="ml-3">
          <DropdownToggle
            tag="a"
            href="javascript:;"
            class="w-5 h-5 text-slate-500"
          >
            <MoreVerticalIcon class="w-5 h-5" />
          </DropdownToggle>
          <DropdownMenu class="w-40">
            <DropdownContent>
              <DropdownItem>
                <Edit2Icon class="w-4 h-4 mr-2" /> Edit Post
              </DropdownItem>
              <DropdownItem>
                <TrashIcon class="w-4 h-4 mr-2" /> Delete Post
              </DropdownItem>
            </DropdownContent>
          </DropdownMenu>
        </Dropdown>
      </div>
      <div class="p-5">
        <div class="h-40 2xl:h-56 image-fit">
          <img
            alt="Icewall Tailwind HTML Admin Template"
            class="rounded-md"
            :src="faker.images[0]"
          />
        </div>
        <a href="" class="block font-medium text-base mt-5">{{
          faker.news[0].title
        }}</a>
        <div class="text-slate-600 dark:text-slate-500 mt-2">
          {{ faker.news[0].shortContent }}
        </div>
      </div>
      <div
        class="flex items-center px-5 py-3 border-t border-slate-200/60 dark:border-darkmode-400"
      >
        <Tippy
          tag="a"
          href=""
          class="intro-x w-8 h-8 flex items-center justify-center rounded-full border border-slate-300 dark:border-darkmode-400 dark:bg-darkmode-300 dark:text-slate-300 text-slate-500 mr-2"
          content="Bookmark"
        >
          <BookmarkIcon class="w-3 h-3" />
        </Tippy>
        <div class="intro-x flex mr-2">
          <div class="intro-x w-8 h-8 image-fit">
            <Tippy
              tag="img"
              alt="Icewall Tailwind HTML Admin Template"
              class="rounded-full border border-white zoom-in"
              :src="faker.photos[0]"
              :content="faker.users[0].name"
            />
          </div>
          <div class="intro-x w-8 h-8 image-fit -ml-4">
            <Tippy
              tag="img"
              alt="Icewall Tailwind HTML Admin Template"
              class="rounded-full border border-white zoom-in"
              :src="faker.photos[1]"
              :content="faker.users[1].name"
            />
          </div>
          <div class="intro-x w-8 h-8 image-fit -ml-4">
            <Tippy
              tag="img"
              alt="Icewall Tailwind HTML Admin Template"
              class="rounded-full border border-white zoom-in"
              :src="faker.photos[2]"
              :content="faker.users[2].name"
            />
          </div>
        </div>
        <Tippy
          tag="a"
          href=""
          class="intro-x w-8 h-8 flex items-center justify-center rounded-full text-primary bg-primary/10 dark:bg-darkmode-300 dark:text-slate-300 ml-auto"
          content="Share"
        >
          <Share2Icon class="w-3 h-3" />
        </Tippy>
        <Tippy
          tag="a"
          href=""
          class="intro-x w-8 h-8 flex items-center justify-center rounded-full bg-primary text-white ml-2"
          content="Download PDF"
        >
          <ShareIcon class="w-3 h-3" />
        </Tippy>
      </div>
      <div
        class="px-5 pt-3 pb-5 border-t border-slate-200/60 dark:border-darkmode-400"
      >
        <div class="w-full flex text-slate-500 text-xs sm:text-sm">
          <div class="mr-2">
            Comments: <span class="font-medium">{{ faker.totals[0] }}</span>
          </div>
          <div class="mr-2">
            Views: <span class="font-medium">{{ faker.totals[1] }}k</span>
          </div>
          <div class="ml-auto">
            Likes: <span class="font-medium">{{ faker.totals[2] }}k</span>
          </div>
        </div>
        <div class="w-full flex items-center mt-3">
          <div class="w-8 h-8 flex-none image-fit mr-3">
            <img
              alt="Icewall Tailwind HTML Admin Template"
              class="rounded-full"
              :src="faker.photos[0]"
            />
          </div>
          <div class="flex-1 relative text-slate-600">
            <input
              type="text"
              class="form-control form-control-rounded border-transparent bg-slate-100 pr-10"
              placeholder="Post a comment..."
            />
            <SmileIcon
              class="w-4 h-4 absolute my-auto inset-y-0 mr-3 right-0"
            />
          </div>
        </div>
      </div>
    </div>
    <!-- END: Blog Layout -->
    <!-- BEGIN: Pagination -->
    <div
      class="intro-y col-span-12 flex flex-wrap sm:flex-row sm:flex-nowrap items-center"
    >
      <nav class="w-full sm:w-auto sm:mr-auto">
        <ul class="pagination">
          <li class="page-item">
            <a class="page-link" href="#">
              <ChevronsLeftIcon class="w-4 h-4" />
            </a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">
              <ChevronLeftIcon class="w-4 h-4" />
            </a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">...</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">1</a>
          </li>
          <li class="page-item active">
            <a class="page-link" href="#">2</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">3</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">...</a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">
              <ChevronRightIcon class="w-4 h-4" />
            </a>
          </li>
          <li class="page-item">
            <a class="page-link" href="#">
              <ChevronsRightIcon class="w-4 h-4" />
            </a>
          </li>
        </ul>
      </nav>
      <select class="w-20 form-select box mt-3 sm:mt-0">
        <option>10</option>
        <option>25</option>
        <option>35</option>
        <option>50</option>
      </select>
    </div>
    <!-- END: Pagination -->
  </div>
</template>
