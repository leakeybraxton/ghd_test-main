<template>
  <div class="relative">
    <div class="grid grid-cols-12 gap-6">
      <div class="col-span-12 xl:col-span-9 2xl:col-span-9 z-10">
        <div class="mt-6 -mb-6 intro-y">
          <Alert
            class="box bg-primary text-white flex items-center mb-6"
            v-slot="{ dismiss }"
          >
            <span>
              Introducing new dashboard! Download now at
              <a
                href="https://themeforest.net/item/midone-jquery-tailwindcss-html-admin-template/26366820"
                class="underline ml-1"
                target="blank"
                >themeforest.net</a
              >.
              <button
                class="rounded-md bg-white bg-opacity-20 dark:bg-darkmode-300 hover:bg-opacity-30 py-0.5 px-2 -my-3 ml-2"
              >
                Live Preview
              </button>
            </span>
            <button
              type="button"
              class="btn-close text-white"
              @click="dismiss"
              aria-label="Close"
            >
              <XIcon class="w-4 h-4" />
            </button>
          </Alert>
        </div>
        <div class="mt-14 mb-3 grid grid-cols-12 sm:gap-10 intro-y">
          <div
            class="col-span-12 sm:col-span-6 md:col-span-4 py-6 sm:pl-5 md:pl-0 lg:pl-5 relative text-center sm:text-left"
          >
            <Dropdown
              class="absolute pt-0.5 2xl:pt-0 mt-5 2xl:mt-6 top-0 right-0"
            >
              <DropdownToggle tag="a" class="block" href="javascript:;">
                <MoreVerticalIcon class="w-5 h-5 text-slate-500" />
              </DropdownToggle>
              <DropdownMenu class="w-40">
                <DropdownContent>
                  <DropdownItem>
                    <FileTextIcon class="w-4 h-4 mr-2" />
                    Monthly Report
                  </DropdownItem>
                  <DropdownItem>
                    <FileTextIcon class="w-4 h-4 mr-2" />
                    Annual Report
                  </DropdownItem>
                </DropdownContent>
              </DropdownMenu>
            </Dropdown>
            <div class="text-sm 2xl:text-base font-medium -mb-1">
              Hi Angelina,
              <span class="text-slate-600 dark:text-slate-300 font-normal"
                >welcome back!</span
              >
            </div>
            <div
              class="text-base 2xl:text-lg justify-center sm:justify-start flex items-center text-slate-600 dark:text-slate-300 leading-3 mt-14 2xl:mt-24"
            >
              My Total Assets
              <Tippy
                tag="div"
                content="Total value of your sales: $158.409.416"
              >
                <AlertCircleIcon class="w-5 h-5 ml-1.5 mt-0.5" />
              </Tippy>
            </div>
            <div class="2xl:flex mt-5 mb-3">
              <div class="flex items-center justify-center sm:justify-start">
                <div
                  class="relative text-2xl 2xl:text-3xl font-medium leading-6 pl-3 2xl:pl-4"
                >
                  <span
                    class="absolute text-xl 2xl:text-2xl top-0 left-0 -mt-1 2xl:mt-0"
                    >$</span
                  >
                  142,402,210
                </div>
                <a class="text-slate-500 ml-4 2xl:ml-16" href="">
                  <RefreshCcwIcon class="w-4 h-4" />
                </a>
              </div>
              <div
                class="mt-5 2xl:flex 2xl:justify-center 2xl:mt-0 2xl:-ml-20 2xl:w-14 2xl:flex-none 2xl:pl-2.5"
              >
                <Tippy
                  tag="div"
                  class="font-medium inline-flex bg-success text-white rounded-full px-2 py-1 text-xs 2xl:text-sm 2xl:p-0 2xl:text-success 2xl:bg-transparent 2xl:flex items-center cursor-pointer 2xl:justify-center"
                  content="49% Higher than last month"
                >
                  49%
                  <ChevronUpIcon class="w-4 h-4 ml-0.5" />
                </Tippy>
              </div>
            </div>
            <div class="text-slate-500">Last updated 1 hour ago</div>
            <div
              class="2xl:text-base text-slate-600 dark:text-slate-300 mt-6 -mb-1"
            >
              Total net margin
              <a
                href=""
                class="underline decoration-dotted underline-offset-4 text-primary dark:text-slate-400"
                >$12,921,050</a
              >
            </div>
            <Dropdown class="mt-14 2xl:mt-24">
              <DropdownToggle
                class="btn btn-rounded-primary w-44 2xl:w-52 px-4 relative justify-start"
              >
                Download Reports
                <span
                  class="w-8 h-8 absolute flex justify-center items-center right-0 top-0 bottom-0 my-auto ml-auto mr-1"
                >
                  <ChevronDownIcon class="w-4 h-4" />
                </span>
              </DropdownToggle>
              <DropdownMenu class="w-44 2xl:w-52">
                <DropdownContent>
                  <DropdownItem>
                    <FileTextIcon class="w-4 h-4 mr-2" />
                    Monthly Report
                  </DropdownItem>
                  <DropdownItem>
                    <FileTextIcon class="w-4 h-4 mr-2" />
                    Annual Report
                  </DropdownItem>
                </DropdownContent>
              </DropdownMenu>
            </Dropdown>
          </div>
          <div
            class="row-start-2 md:row-start-auto col-span-12 md:col-span-4 py-6 border-black border-opacity-10 border-t md:border-t-0 md:border-l md:border-r border-dashed px-10 sm:px-28 md:px-5 -mx-5"
          >
            <div class="flex flex-wrap items-center">
              <div
                class="flex items-center w-full sm:w-auto justify-center sm:justify-start mr-auto mb-5 2xl:mb-0"
              >
                <div class="w-2 h-2 bg-primary rounded-full -mt-4"></div>
                <div class="ml-3.5">
                  <div
                    class="relative text-xl 2xl:text-2xl font-medium leading-6 2xl:leading-5 pl-3.5 2xl:pl-4"
                  >
                    <span
                      class="absolute text-base 2xl:text-xl top-0 left-0 2xl:-mt-1.5"
                      >$</span
                    >
                    47,578.77
                  </div>
                  <div class="text-slate-500 mt-2">Yearly budget</div>
                </div>
              </div>
              <select
                class="form-select bg-transparent border-black border-opacity-10 dark:border-darkmode-400 dark:bg-transparent mx-auto sm:mx-0 py-1.5 px-3 w-auto -mt-2"
              >
                <option value="daily">Daily</option>
                <option value="weekly">Weekly</option>
                <option value="monthly">Monthly</option>
                <option value="yearly">Yearly</option>
                <option value="custom-date">Custom Date</option>
              </select>
            </div>
            <div class="mt-10 text-slate-600 dark:text-slate-300">
              You have spent about 35% of your annual budget.
            </div>
            <div class="mt-6">
              <ReportBarChart1 :height="290" />
            </div>
          </div>
          <TabGroup
            class="col-span-12 sm:col-span-6 md:col-span-4 py-6 border-black border-opacity-10 border-t sm:border-t-0 border-l md:border-l-0 border-dashed -ml-4 pl-4 md:ml-0 md:pl-0"
          >
            <TabList
              class="nav-pills w-3/4 2xl:w-4/6 bg-slate-200 dark:bg-black/10 rounded-md mx-auto p-1"
            >
              <Tab class="w-full py-1.5 px-2" tag="button">Active</Tab>
              <Tab class="w-full py-1.5 px-2" tag="button">Inactive</Tab>
            </TabList>
            <TabPanels class="mt-6">
              <TabPanel>
                <div class="relative">
                  <ReportDonutChart2 :height="212" class="mt-8" />
                  <div
                    class="flex flex-col justify-center items-center absolute w-full h-full top-0 left-0"
                  >
                    <div class="text-xl 2xl:text-2xl font-medium">2.501</div>
                    <div class="text-slate-500 mt-0.5">Active Users</div>
                  </div>
                </div>
                <div class="mx-auto w-10/12 2xl:w-2/3 mt-8">
                  <div class="flex items-center">
                    <div class="w-2 h-2 bg-primary rounded-full mr-3"></div>
                    <span class="truncate">17 - 30 Years old</span>
                    <span class="font-medium xl:ml-auto">62%</span>
                  </div>
                  <div class="flex items-center mt-4">
                    <div class="w-2 h-2 bg-pending rounded-full mr-3"></div>
                    <span class="truncate">31 - 50 Years old</span>
                    <span class="font-medium xl:ml-auto">33%</span>
                  </div>
                  <div class="flex items-center mt-4">
                    <div class="w-2 h-2 bg-warning rounded-full mr-3"></div>
                    <span class="truncate">>= 50 Years old</span>
                    <span class="font-medium xl:ml-auto">10%</span>
                  </div>
                </div>
              </TabPanel>
            </TabPanels>
          </TabGroup>
        </div>
      </div>
      <div class="report-box-3 px-5 pt-8 pb-14 col-span-12 z-10">
        <div class="grid grid-cols-12 gap-6 relative intro-y">
          <div
            class="col-span-12 sm:col-span-4 xl:col-span-3 px-0 lg:px-6 xl:px-0 2xl:px-6"
          >
            <div class="flex items-center flex-wrap lg:flex-nowrap gap-3">
              <div
                class="sm:w-full lg:w-auto text-lg font-medium truncate mr-auto"
              >
                Summary Report
              </div>
              <div
                class="py-1 px-2.5 rounded-full text-xs bg-slate-300/50 dark:bg-darkmode-400 text-slate-600 dark:text-slate-300 cursor-pointer truncate"
              >
                180 Campaign
              </div>
            </div>
            <div class="px-10 sm:px-0">
              <SimpleLineChart3 :height="110" class="mt-8" />
            </div>
          </div>
          <div
            class="col-span-12 sm:col-span-4 xl:col-span-3 px-0 lg:px-6 xl:px-0 2xl:px-6"
          >
            <div class="flex items-center flex-wrap lg:flex-nowrap gap-3">
              <div
                class="sm:w-full lg:w-auto text-lg font-medium truncate mr-auto"
              >
                Social Media
              </div>
              <a href="" class="flex items-center text-primary">
                <div class="truncate 2xl:mr-auto">View Details</div>
                <ArrowRightIcon class="w-4 h-4 ml-3" />
              </a>
            </div>
            <div class="flex items-center justify-center mt-10">
              <div class="text-right">
                <div class="text-3xl font-medium">149</div>
                <div class="truncate mt-1 text-slate-500">Active Lenders</div>
              </div>
              <div
                class="w-px h-16 border border-r border-dashed border-slate-300 dark:border-darkmode-400 mx-4 xl:mx-6"
              ></div>
              <div>
                <div class="text-3xl font-medium">135</div>
                <div class="truncate mt-1 text-slate-500">Total Lenders</div>
              </div>
            </div>
          </div>
          <div
            class="col-span-12 sm:col-span-4 xl:col-span-3 px-0 lg:px-6 xl:px-0 2xl:px-6"
          >
            <div class="flex items-center flex-wrap lg:flex-nowrap gap-3">
              <div
                class="sm:w-full lg:w-auto text-lg font-medium truncate mr-auto"
              >
                Posted Ads
              </div>
              <div
                class="py-1 px-2.5 rounded-full text-xs bg-slate-300/50 dark:bg-darkmode-400 text-slate-600 dark:text-slate-300 cursor-pointer truncate"
              >
                320 Followers
              </div>
            </div>
            <div class="px-10 sm:px-0">
              <SimpleLineChart4 :height="110" class="mt-8" />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div
      class="report-box-4 w-full h-full grid grid-cols-12 gap-6 xl:absolute -mt-8 xl:mt-0 pb-6 xl:pb-0 top-0 right-0 z-30 xl:z-auto"
    >
      <div class="col-span-12 xl:col-span-3 xl:col-start-10 xl:pb-16 z-30">
        <div class="h-full flex flex-col">
          <div class="box p-5 mt-6 bg-primary intro-x">
            <div class="flex flex-wrap gap-3">
              <div class="mr-auto">
                <div
                  class="text-white text-opacity-70 dark:text-slate-300 flex items-center leading-3"
                >
                  AVAILABLE FUNDS
                  <Tippy
                    tag="div"
                    content="Total value of your sales: $158.409.416"
                  >
                    <AlertCircleIcon class="w-4 h-4 ml-1.5" />
                  </Tippy>
                </div>
                <div
                  class="text-white relative text-2xl font-medium leading-5 pl-4 mt-3.5"
                >
                  <span class="absolute text-xl top-0 left-0 -mt-1.5">$</span>
                  479,578.77
                </div>
              </div>
              <a
                class="flex items-center justify-center w-12 h-12 rounded-full bg-white dark:bg-darkmode-300 bg-opacity-20 hover:bg-opacity-30 text-white"
                href=""
              >
                <PlusIcon class="w-6 h-6" />
              </a>
            </div>
          </div>
          <div class="report-box-4__content xl:min-h-0 intro-x">
            <TabGroup class="max-h-full xl:overflow-y-auto box mt-5">
              <div class="xl:sticky top-0 px-5 pt-5 pb-6">
                <div class="flex items-center">
                  <div class="text-lg font-medium truncate mr-5">
                    Summary Report
                  </div>
                  <a href="" class="ml-auto flex items-center text-primary">
                    <RefreshCcwIcon class="w-4 h-4 mr-3" />
                    Refresh
                  </a>
                </div>
                <TabList
                  class="nav-pills border border-slate-300 dark:border-darkmode-300 border-dashed rounded-md mx-auto p-1 mt-5"
                >
                  <Tab class="w-full py-1.5 px-2 active" tag="button"
                    >Weekly</Tab
                  >
                  <Tab class="w-full py-1.5 px-2" tag="button">Monthly</Tab>
                </TabList>
              </div>
              <TabPanels class="px-5 pb-5">
                <TabPanel class="grid grid-cols-12 gap-y-6">
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Unpaid Loan</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">$155.430.000</div>
                      <Tippy
                        tag="div"
                        class="text-danger flex text-xs font-medium cursor-pointer ml-2"
                        content="2% Lower than last month"
                      >
                        2%
                        <ChevronDownIcon class="w-4 h-4 ml-0.5" />
                      </Tippy>
                    </div>
                  </div>
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Active Funding Partner</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">52 Partner</div>
                      <Tippy
                        tag="div"
                        class="text-success flex text-xs font-medium tooltip cursor-pointer ml-2"
                        content="0.1% Lower than last month"
                      >
                        49%
                        <ChevronUpIcon class="w-4 h-4 ml-0.5" />
                      </Tippy>
                    </div>
                  </div>
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Paid Installment</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">$75.430.000</div>
                      <Tippy
                        tag="div"
                        class="text-success flex text-xs font-medium tooltip cursor-pointer ml-2"
                        content="49% Higher than last month"
                      >
                        36%
                        <ChevronUpIcon class="w-4 h-4 ml-0.5" />
                      </Tippy>
                    </div>
                  </div>
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Success Payment</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">100%</div>
                    </div>
                  </div>
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Waiting For Disbursement</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">0</div>
                    </div>
                  </div>
                  <div
                    class="col-span-12 sm:col-span-6 md:col-span-4 xl:col-span-12"
                  >
                    <div class="text-slate-500">Unpaid Loan</div>
                    <div class="mt-1.5 flex items-center">
                      <div class="text-lg">$21.430.000</div>
                      <Tippy
                        tag="div"
                        class="text-danger flex text-xs font-medium cursor-pointer ml-2"
                        content="2% Lower than last month"
                      >
                        23%
                        <ChevronDownIcon class="w-4 h-4 ml-0.5" />
                      </Tippy>
                    </div>
                  </div>
                  <button
                    class="btn btn-outline-secondary col-span-12 border-slate-300 dark:border-darkmode-300 border-dashed relative justify-start mb-2"
                  >
                    <span class="truncate mr-5">My Portfolio Details</span>
                    <span
                      class="w-8 h-8 absolute flex justify-center items-center right-0 top-0 bottom-0 my-auto ml-auto mr-0.5"
                    >
                      <ArrowRightIcon class="w-4 h-4" />
                    </span>
                  </button>
                </TabPanel>
              </TabPanels>
            </TabGroup>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div
    class="report-box-3 report-box-3--content grid grid-cols-12 gap-6 xl:-mt-5 2xl:-mt-8 -mb-10 z-40 2xl:z-10"
  >
    <div class="col-span-12 2xl:col-span-9">
      <div class="grid grid-cols-12 gap-6">
        <!-- BEGIN: Official Store -->
        <div class="col-span-12 xl:col-span-8 mt-6">
          <div class="intro-y block sm:flex items-center h-10">
            <h2 class="text-lg font-medium truncate mr-5">Official Store</h2>
            <div class="sm:ml-auto mt-3 sm:mt-0 relative text-slate-500">
              <MapPinIcon
                class="w-4 h-4 z-10 absolute my-auto inset-y-0 ml-3 left-0"
              />
              <input
                type="text"
                class="form-control sm:w-56 box pl-10"
                placeholder="Filter by city"
              />
            </div>
          </div>
          <div class="intro-y box p-5 mt-12 sm:mt-5">
            <div>
              250 Official stores in 21 countries, click the marker to see
              location details.
            </div>
            <ReportMap class="report-maps mt-5 bg-slate-200 rounded-md" />
          </div>
        </div>
        <!-- END: Official Store -->
        <!-- BEGIN: Weekly Best Sellers -->
        <div class="col-span-12 xl:col-span-4 mt-6">
          <div class="intro-y flex items-center h-10">
            <h2 class="text-lg font-medium truncate mr-5">
              Weekly Best Sellers
            </h2>
          </div>
          <div class="mt-5">
            <div
              v-for="(faker, fakerKey) in $_.take($f(), 4)"
              :key="fakerKey"
              class="intro-y"
            >
              <div class="box px-4 py-4 mb-3 flex items-center zoom-in">
                <div
                  class="w-10 h-10 flex-none image-fit rounded-md overflow-hidden"
                >
                  <img
                    alt="Icewall Tailwind HTML Admin Template"
                    :src="faker.photos[0]"
                  />
                </div>
                <div class="ml-4 mr-auto">
                  <div class="font-medium">
                    {{ faker.users[0].name }}
                  </div>
                  <div class="text-slate-500 text-xs mt-0.5">
                    {{ faker.dates[0] }}
                  </div>
                </div>
                <div
                  class="py-1 px-2 rounded-full text-xs bg-success text-white cursor-pointer font-medium"
                >
                  137 Sales
                </div>
              </div>
            </div>
            <a
              href=""
              class="intro-y w-full block text-center rounded-md py-4 border border-dotted border-slate-400 dark:border-darkmode-300 text-slate-500"
              >View More</a
            >
          </div>
        </div>
        <!-- END: Weekly Best Sellers -->
        <!-- BEGIN: Weekly Top Products -->
        <div class="col-span-12 mt-6">
          <div class="intro-y block sm:flex items-center h-10">
            <h2 class="text-lg font-medium truncate mr-5">
              Weekly Top Products
            </h2>
            <div class="flex items-center sm:ml-auto mt-3 sm:mt-0">
              <button
                class="btn box flex items-center text-slate-600 dark:text-slate-300"
              >
                <FileTextIcon class="hidden sm:block w-4 h-4 mr-2" />
                Export to Excel
              </button>
              <button
                class="ml-3 btn box flex items-center text-slate-600 dark:text-slate-300"
              >
                <FileTextIcon class="hidden sm:block w-4 h-4 mr-2" />
                Export to PDF
              </button>
            </div>
          </div>
          <div class="intro-y overflow-auto lg:overflow-visible mt-8 sm:mt-0">
            <table class="table table-report sm:mt-2">
              <thead>
                <tr>
                  <th class="whitespace-nowrap">IMAGES</th>
                  <th class="whitespace-nowrap">PRODUCT NAME</th>
                  <th class="text-center whitespace-nowrap">STOCK</th>
                  <th class="text-center whitespace-nowrap">STATUS</th>
                  <th class="text-center whitespace-nowrap">ACTIONS</th>
                </tr>
              </thead>
              <tbody>
                <tr
                  v-for="(faker, fakerKey) in $_.take($f(), 4)"
                  :key="fakerKey"
                  class="intro-x"
                >
                  <td class="w-40">
                    <div class="flex">
                      <div class="w-10 h-10 image-fit zoom-in">
                        <Tippy
                          tag="img"
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-full"
                          :src="faker.images[0]"
                          :content="`Uploaded at ${faker.dates[0]}`"
                        />
                      </div>
                      <div class="w-10 h-10 image-fit zoom-in -ml-5">
                        <Tippy
                          tag="img"
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-full"
                          :src="faker.images[1]"
                          :content="`Uploaded at ${faker.dates[1]}`"
                        />
                      </div>
                      <div class="w-10 h-10 image-fit zoom-in -ml-5">
                        <Tippy
                          tag="img"
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-full"
                          :src="faker.images[2]"
                          :content="`Uploaded at ${faker.dates[2]}`"
                        />
                      </div>
                    </div>
                  </td>
                  <td>
                    <a href="" class="font-medium whitespace-nowrap">{{
                      faker.products[0].name
                    }}</a>
                    <div
                      class="text-slate-500 text-xs whitespace-nowrap mt-0.5"
                    >
                      {{ faker.products[0].category }}
                    </div>
                  </td>
                  <td class="text-center">{{ faker.stocks[0] }}</td>
                  <td class="w-40">
                    <div
                      class="flex items-center justify-center"
                      :class="{
                        'text-success': faker.trueFalse[0],
                        'text-danger': !faker.trueFalse[0],
                      }"
                    >
                      <CheckSquareIcon class="w-4 h-4 mr-2" />
                      {{ faker.trueFalse[0] ? "Active" : "Inactive" }}
                    </div>
                  </td>
                  <td class="table-report__action w-56">
                    <div class="flex justify-center items-center">
                      <a class="flex items-center mr-3" href="">
                        <CheckSquareIcon class="w-4 h-4 mr-1" />
                        Edit
                      </a>
                      <a class="flex items-center text-danger" href="">
                        <Trash2Icon class="w-4 h-4 mr-1" /> Delete
                      </a>
                    </div>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
          <div
            class="intro-y flex flex-wrap sm:flex-row sm:flex-nowrap items-center mt-3"
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
        </div>
        <!-- END: Weekly Top Products -->
      </div>
    </div>
    <div class="col-span-12 2xl:col-span-3 relative z-10">
      <div class="2xl:border-l pb-10 intro-y">
        <div class="2xl:pl-6 grid grid-cols-12 gap-x-6 2xl:gap-x-0 gap-y-6">
          <!-- BEGIN: Recent Activities -->
          <div
            class="col-span-12 md:col-span-6 xl:col-span-4 2xl:col-span-12 mt-3"
          >
            <div class="intro-x flex items-center h-10">
              <h2 class="text-lg font-medium truncate mr-5">
                Recent Activities
              </h2>
              <a href="" class="ml-auto text-primary truncate">Show More</a>
            </div>
            <div
              class="mt-5 relative before:block before:absolute before:w-px before:h-[85%] before:bg-slate-200 before:dark:bg-darkmode-400 before:ml-5 before:mt-5"
            >
              <div class="intro-x relative flex items-center mb-3">
                <div
                  class="before:block before:absolute before:w-20 before:h-px before:bg-slate-200 before:dark:bg-darkmode-400 before:mt-5 before:ml-5"
                >
                  <div
                    class="w-10 h-10 flex-none image-fit rounded-full overflow-hidden"
                  >
                    <img
                      alt="Icewall Tailwind HTML Admin Template"
                      :src="$f()[9].photos[0]"
                    />
                  </div>
                </div>
                <div class="box px-5 py-3 ml-4 flex-1 zoom-in">
                  <div class="flex items-center">
                    <div class="font-medium">
                      {{ $f()[9].users[0].name }}
                    </div>
                    <div class="text-xs text-slate-500 ml-auto">07:00 PM</div>
                  </div>
                  <div class="text-slate-500 mt-1">Has joined the team</div>
                </div>
              </div>
              <div class="intro-x relative flex items-center mb-3">
                <div
                  class="before:block before:absolute before:w-20 before:h-px before:bg-slate-200 before:dark:bg-darkmode-400 before:mt-5 before:ml-5"
                >
                  <div
                    class="w-10 h-10 flex-none image-fit rounded-full overflow-hidden"
                  >
                    <img
                      alt="Icewall Tailwind HTML Admin Template"
                      :src="$f()[8].photos[0]"
                    />
                  </div>
                </div>
                <div class="box px-5 py-3 ml-4 flex-1 zoom-in">
                  <div class="flex items-center">
                    <div class="font-medium">
                      {{ $f()[8].users[0].name }}
                    </div>
                    <div class="text-xs text-slate-500 ml-auto">07:00 PM</div>
                  </div>
                  <div class="text-slate-500">
                    <div class="mt-1">Added 3 new photos</div>
                    <div class="flex mt-2">
                      <Tippy
                        tag="div"
                        class="w-8 h-8 image-fit mr-1 zoom-in"
                        :content="$f()[0].products[0].name"
                      >
                        <img
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-md border border-white"
                          :src="$f()[8].images[0]"
                        />
                      </Tippy>
                      <Tippy
                        tag="div"
                        class="w-8 h-8 image-fit mr-1 zoom-in"
                        :content="$f()[1].products[0].name"
                      >
                        <img
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-md border border-white"
                          :src="$f()[8].images[1]"
                        />
                      </Tippy>
                      <Tippy
                        tag="div"
                        class="w-8 h-8 image-fit mr-1 zoom-in"
                        :content="$f()[2].products[0].name"
                      >
                        <img
                          alt="Icewall Tailwind HTML Admin Template"
                          class="rounded-md border border-white"
                          :src="$f()[8].images[2]"
                        />
                      </Tippy>
                    </div>
                  </div>
                </div>
              </div>
              <div class="intro-x text-slate-500 text-xs text-center my-4">
                12 November
              </div>
              <div class="intro-x relative flex items-center mb-3">
                <div
                  class="before:block before:absolute before:w-20 before:h-px before:bg-slate-200 before:dark:bg-darkmode-400 before:mt-5 before:ml-5"
                >
                  <div
                    class="w-10 h-10 flex-none image-fit rounded-full overflow-hidden"
                  >
                    <img
                      alt="Icewall Tailwind HTML Admin Template"
                      :src="$f()[7].photos[0]"
                    />
                  </div>
                </div>
                <div class="box px-5 py-3 ml-4 flex-1 zoom-in">
                  <div class="flex items-center">
                    <div class="font-medium">
                      {{ $f()[7].users[0].name }}
                    </div>
                    <div class="text-xs text-slate-500 ml-auto">07:00 PM</div>
                  </div>
                  <div class="text-slate-500 mt-1">
                    Has changed
                    <a class="text-primary" href="">{{
                      $f()[7].products[0].name
                    }}</a>
                    price and description
                  </div>
                </div>
              </div>
              <div class="intro-x relative flex items-center mb-3">
                <div
                  class="before:block before:absolute before:w-20 before:h-px before:bg-slate-200 before:dark:bg-darkmode-400 before:mt-5 before:ml-5"
                >
                  <div
                    class="w-10 h-10 flex-none image-fit rounded-full overflow-hidden"
                  >
                    <img
                      alt="Icewall Tailwind HTML Admin Template"
                      :src="$f()[6].photos[0]"
                    />
                  </div>
                </div>
                <div class="box px-5 py-3 ml-4 flex-1 zoom-in">
                  <div class="flex items-center">
                    <div class="font-medium">
                      {{ $f()[6].users[0].name }}
                    </div>
                    <div class="text-xs text-slate-500 ml-auto">07:00 PM</div>
                  </div>
                  <div class="text-slate-500 mt-1">
                    Has changed
                    <a class="text-primary" href="">{{
                      $f()[6].products[0].name
                    }}</a>
                    description
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- END: Recent Activities -->
          <!-- BEGIN: Transactions -->
          <div
            class="col-span-12 md:col-span-6 xl:col-span-4 2xl:col-span-12 mt-3"
          >
            <div class="intro-x flex items-center h-10">
              <h2 class="text-lg font-medium truncate mr-5">Transactions</h2>
            </div>
            <div class="mt-5">
              <div
                v-for="(faker, fakerKey) in $_.take($f(), 5)"
                :key="fakerKey"
                class="intro-x"
              >
                <div class="box px-5 py-3 mb-3 flex items-center zoom-in">
                  <div
                    class="w-10 h-10 flex-none image-fit rounded-full overflow-hidden"
                  >
                    <img
                      alt="Icewall Tailwind HTML Admin Template"
                      :src="faker.photos[0]"
                    />
                  </div>
                  <div class="ml-4 mr-auto">
                    <div class="font-medium">
                      {{ faker.users[0].name }}
                    </div>
                    <div class="text-slate-500 text-xs mt-0.5">
                      {{ faker.dates[0] }}
                    </div>
                  </div>
                  <div
                    :class="{
                      'text-success': faker.trueFalse[0],
                      'text-danger': !faker.trueFalse[0],
                    }"
                  >
                    {{ faker.trueFalse[0] ? "+" : "-" }}${{ faker.totals[0] }}
                  </div>
                </div>
              </div>
              <a
                href=""
                class="intro-x w-full block text-center rounded-md py-3 border border-dotted border-slate-400 dark:border-darkmode-300 text-slate-500"
                >View More</a
              >
            </div>
          </div>
          <!-- END: Transactions -->
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import ReportDonutChart2 from "@/components/report-donut-chart-2/Main.vue";
import ReportBarChart1 from "@/components/report-bar-chart-1/Main.vue";
import ReportMap from "@/components/report-map/Main.vue";
import SimpleLineChart3 from "@/components/simple-line-chart-3/Main.vue";
import SimpleLineChart4 from "@/components/simple-line-chart-4/Main.vue";
</script>
