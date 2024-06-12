# tailwindcss
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100">
    <!-- Side bar  min-height:100%vh, display:none md:min-width:768px-->
     <!-- hidden md:block(media screemn) -->
      <!-- https://jsfiddel.net/ufhar56d/32 -->
    <div class="flex min-h-[100vh] flex-no-wrap">
        <div class="w-64 bg-gray-800 hidden md:block">
            <!-- Dashboard text wrapper -->
            <div class="flex justify-center items-center h-20 bg-gray-900">
                <h1 class="text-white text-2xl">DashBoard</h1>
            </div>

            <nav class="mt-10">
                <a href="#" class="flex mt-4 items-center py-2 px-6 bg-gray-700 text-gray-100 hover:text-gray-400">
                    <span class="mx-3">Home</span>
                </a>
                <a href="#" class="flex mt-4 items-center py-2 px-6 hover:bg-gray-700 text-gray-100 hover:text-gray-400">
                    <span class="mx-3">Analytics</span>
                </a>

                <a href="#" class="flex mt-4 items-center py-2 px-6 hover:bg-gray-700 text-gray-100 hover:text-gray-400">
                    <span class="mx-3">Sales</span>
                </a>

                <a href="#" class="flex mt-4 items-center py-2 px-6 hover:bg-gray-700 text-gray-100 hover:text-gray-400">
                    <span class="mx-3">Messages</span>
                </a>
                
            </nav>

        </div>

        <!-- main content -->
        <div class="flex flex-col w-full">
            <!-- nav bar -->
             <!-- md:hidden when width more or equal than md:block -->
              
             <header class="flex items-center bg-white px-4 h-16">
                <!-- Sidebar button -->
                <button class="md:hidden px-4 py-2 border rounded-md text-gray-600 border-gray-300 hover:text-gray-300">
                    <svg class="h-6 w-6" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M4 18H10" stroke="#000000" stroke-width="2" stroke-linecap="round"/>
                        <path d="M4 12L16 12" stroke="#000000" stroke-width="2" stroke-linecap="round"/>
                        <path d="M4 6L20 6" stroke="#000000" stroke-width="2" stroke-linecap="round"/>
                    </svg>
                </button>

                <div class="ml-auto flex items-center">
                    <button class="flex items-center px-4 py-2 border rounded-md text-gray-600 border-gray-300">
                        <span class="mr-2">Sign out</span>
                    </button>
                </div>
             </header>

             <!-- content -->
              <main class="p-4 md:p-6">
                <!-- card warpper -->
                <div class="flex flex-wrap gap-5">
                    <!-- card UI -->
                     <div class="bg-white p-4 md:p-6 rounded-lg shadow-lg min-w-[40%] transition-shadow duration-300 ease-in-out hover:shadow-none">
                        <h3 class="text-xl fint-semibold mb-4">Revenue</h3>
                        <p class="text-gray-600 text-3xl">$12000</p>
                     </div>
                     <div class="bg-white p-4 md:p-6 rounded-lg shadow-lg min-w-[40%] transition-shadow duration-300 ease-in-out hover:shadow-none">
                        <h3 class="text-xl fint-semibold mb-4">Users</h3>
                        <p class="text-gray-600 text-3xl">$5000</p>
                     </div>
                     <div class="bg-white p-4 md:p-6 rounded-lg shadow-lg min-w-[40%] transition-shadow duration-300 ease-in-out hover:shadow-none">
                        <h3 class="text-xl fint-semibold mb-4">Sales</h3>
                        <p class="text-gray-600 text-3xl">$4512</p>
                     </div>
                </div>

                <div class="mt-8">
                    <div class="flex items-center justify-between">
                        <h2 class="text-xl font-semi-bold">Recent activities</h2>
                        <button class="py-2 px-4 bg-blue-600 text-white rounded-lg hover:bg-blue-700">View All</button>
                    </div>

                    <div class="bg-white p-4 md:p-6 rounded-lg shadow-lg mt-4 overflow-x-auto">
                        <!-- w-full -->
                        <table class="w-[100%]">
                            <thead>
                                <tr class="text-left border-b">
                                    <th class="py-2">Date</th>
                                    <th class="py-2">Activity</th>
                                    <th class="py-2">Status</th>
                                </tr>
                            </thead>

                            <tbody>
                                <tr class="border-b">
                                    <td class="py-2">01/01/2024</td>
                                    <td class="py-2">Logged In</td>
                                    <td class="py-2 text-green-600">Completed</td>
                                </tr>
                                <tr class="border-b">
                                    <td class="py-2">01/01/2024</td>
                                    <td class="py-2">Logged In</td>
                                    <td class="py-2 text-green-600">Completed</td>
                                </tr>
                                <tr class="border-b">
                                    <td class="py-2">01/01/2024</td>
                                    <td class="py-2">Logged In</td>
                                    <td class="py-2 text-green-600">Completed</td>
                                </tr>
                                <tr class="border-b">
                                    <td class="py-2">01/01/2024</td>
                                    <td class="py-2">Logged In</td>
                                    <td class="py-2 text-green-600">Completed</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    
                    <div class="bg-white p-4 md:p-6 rounded-lg shadow-lg h-64 mt-8">
                        <h3 class="text-xl font-semi-bold">Activity feed</h3>

                        <div class="overflow-y-scroll h-[80%]">
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-red-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-green-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                            <div class="flex items-center mb-4">
                                <div class="w-10 h-10 rounded-full bg-blue-600 flex items-center justify-center text-white">
                                    JD
                                </div>
    
                                <div class="ml-4">
                                    <p class="font-semibold">John Dow</p>
                                    <p class="text-gray-600">Logged In</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
              </main>
              <!-- Add a footer -->
              <footer class="bg-black h-20 rounded-lg mt-4 py-5 border">
                    <div class="text-2xl text-center text-white">
                         &copy; 2024 My Cab App. All rights reserved.
                    </div>
              </footer>
        </div>
    </div>
</body>
</html>
