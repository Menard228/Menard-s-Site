<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music & Freedom Wall</title>
    <script src="https://cdn.tailwindcss.com/3.4.16"></script>
    <script>tailwind.config={theme:{extend:{colors:{primary:'#0066cc',secondary:'#ff4d4d'},borderRadius:{'none':'0px','sm':'4px',DEFAULT:'8px','md':'12px','lg':'16px','xl':'20px','2xl':'24px','3xl':'32px','full':'9999px','button':'8px'}}}}</script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/remixicon/4.6.0/remixicon.min.css">
    <style>
        :where([class^="ri-"])::before { content: "\f3c2"; }
        .music-progress::-webkit-progress-bar {
            background-color: #e0e0e0;
            border-radius: 4px;
        }
        .music-progress::-webkit-progress-value {
            background-color: #0066cc;
            border-radius: 4px;
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 4px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #0066cc;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">
    <!-- Nav bar -->
    <nav class="bg-primary text-white fixed w-full top-0 z-50 shadow-md">
        <div class="flex justify-between items-center px-4 py-3">
            <div class="flex items-center space-x-2">
                <span class="font-['Pacifico'] text-xl">MENARD'S SITE </span>
            </div>
            <div class="flex items-center space-x-4">
                <button class="w-8 h-8 flex items-center justify-center rounded-full bg-white/20 cursor-pointer">
                    <i class="ri-notification-3-line text-white ri-lg"></i>
                </button>
                <button class="w-8 h-8 flex items-center justify-center rounded-full bg-white/20 cursor-pointer">
                    <i class="ri-settings-3-line text-white ri-lg"></i>
                </button>
                <div class="w-8 h-8 rounded-full bg-white/20 flex items-center justify-center cursor-pointer">
                    <i class="ri-user-line text-white ri-lg"></i>
                </div>
            </div>
        </div>
    </nav>

    <!-- Music Player -->
    <div class="fixed top-[60px] w-full bg-white shadow-md z-40 px-4 py-3">
        <div class="flex items-center justify-between mb-2">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 rounded bg-gray-200 overflow-hidden">
                    <img src="https://readdy.ai/api/search-image?query=abstract%20music%20album%20cover%20art%2C%20minimalist%20design%2C%20blue%20and%20white%20color%20scheme%2C%20geometric%20shapes%2C%20modern%20aesthetic%2C%20high%20quality&width=100&height=100&seq=1&orientation=squarish" alt="Album Cover" class="w-full h-full object-cover">
                </div>
                <div>
                    <p class="text-sm font-medium">Blinding Lights</p>
                    <p class="text-xs text-gray-500">The Weeknd</p>
                </div>
            </div>
            <div class="flex items-center space-x-4">
                <button class="w-8 h-8 flex items-center justify-center cursor-pointer">
                    <i class="ri-skip-back-fill text-primary ri-lg"></i>
                </button>
                <button class="w-10 h-10 flex items-center justify-center bg-primary rounded-full cursor-pointer">
                    <i class="ri-play-fill text-white ri-lg"></i>
                </button>
                <button class="w-8 h-8 flex items-center justify-center cursor-pointer">
                    <i class="ri-skip-forward-fill text-primary ri-lg"></i>
                </button>
            </div>
        </div>
        <div class="flex items-center space-x-2">
            <span class="text-xs">1:45</span>
            <progress class="music-progress flex-1 h-1" value="35" max="100"></progress>
            <span class="text-xs">3:20</span>
            <button class="w-8 h-8 flex items-center justify-center cursor-pointer">
                <i class="ri-volume-up-line text-gray-600"></i>
            </button>
        </div>
    </div>

    <!-- Main Content -->
    <main class="pt-[140px] pb-16 px-4">
        <!-- Freedom Wall Section -->
        <section class="mb-8">
            <div class="flex justify-between items-center mb-4">
                <h2 class="text-lg font-semibold">Freedom Wall</h2>
                <button class="text-sm text-primary">View All</button>
            </div>
            
            <div class="space-y-4 custom-scrollbar" style="max-height: 400px; overflow-y: auto;">
                <!-- Post 1 -->
                <div class="bg-white p-4 rounded-lg shadow-sm">
                    <div class="flex items-start space-x-3 mb-3">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center">
                            <i class="ri-user-line text-primary"></i>
                        </div>
                        <div>
                            <p class="text-sm font-medium">Anonymous</p>
                            <p class="text-xs text-gray-500">June 11, 2025 • 10:23 AM</p>
                        </div>
                    </div>
                    <p class="text-sm mb-3">Just discovered an amazing new band called "Lunar Eclipse" - their new album is absolutely mind-blowing! Anyone else a fan?</p>
                    <div class="flex items-center space-x-4 text-xs text-gray-500">
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-heart-line"></i>
                            <span>24</span>
                        </button>
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-chat-1-line"></i>
                            <span>8</span>
                        </button>
                    </div>
                </div>
                
                <!-- Post 2 -->
                <div class="bg-white p-4 rounded-lg shadow-sm">
                    <div class="flex items-start space-x-3 mb-3">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center">
                            <i class="ri-user-line text-primary"></i>
                        </div>
                        <div>
                            <p class="text-sm font-medium">MusicLover92</p>
                            <p class="text-xs text-gray-500">June 11, 2025 • 9:15 AM</p>
                        </div>
                    </div>
                    <p class="text-sm mb-3">Anyone else excited for the Twenty One Pilots concert next month? I've been waiting for years to see them live!</p>
                    <div class="h-40 bg-gray-100 rounded mb-3 overflow-hidden">
                        <img src="https://readdy.ai/api/search-image?query=concert%20crowd%2C%20enthusiastic%20fans%2C%20concert%20venue%2C%20stage%20lights%2C%20vibrant%20atmosphere%2C%20high%20energy%2C%20concert%20photography%2C%20wide%20shot%2C%20no%20faces%20visible&width=320&height=160&seq=2&orientation=landscape" alt="Concert" class="w-full h-full object-cover object-top">
                    </div>
                    <div class="flex items-center space-x-4 text-xs text-gray-500">
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-heart-line"></i>
                            <span>42</span>
                        </button>
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-chat-1-line"></i>
                            <span>15</span>
                        </button>
                    </div>
                </div>
                
                <!-- Post 3 -->
                <div class="bg-white p-4 rounded-lg shadow-sm">
                    <div class="flex items-start space-x-3 mb-3">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center">
                            <i class="ri-user-line text-primary"></i>
                        </div>
                        <div>
                            <p class="text-sm font-medium">GamingNinja</p>
                            <p class="text-xs text-gray-500">June 10, 2025 • 8:45 PM</p>
                        </div>
                    </div>
                    <p class="text-sm mb-3">Just reached Diamond rank in Valorant! The grind was real but totally worth it. Anyone want to team up this weekend?</p>
                    <div class="flex items-center space-x-4 text-xs text-gray-500">
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-heart-line"></i>
                            <span>18</span>
                        </button>
                        <button class="flex items-center space-x-1 cursor-pointer">
                            <i class="ri-chat-1-line"></i>
                            <span>6</span>
                        </button>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- My Favorite Games -->
        <section class="mb-8">
            <div class="flex justify-between items-center mb-4">
                <h2 class="text-lg font-semibold">My Favorite Games</h2>
                <button class="text-sm text-primary cursor-pointer">Customize</button>
            </div>
            
            <div class="grid grid-cols-2 gap-3">
                <div class="bg-white rounded-lg shadow-sm overflow-hidden cursor-pointer">
                    <div class="h-24 bg-gray-200 overflow-hidden">
                        <img src="https://readdy.ai/api/search-image?query=valorant%20game%20screenshot%2C%20tactical%20shooter%20gameplay%2C%20vibrant%20colors%2C%20action%20scene%2C%20no%20faces%20visible&width=160&height=120&seq=3&orientation=landscape" alt="Valorant" class="w-full h-full object-cover object-top">
                    </div>
                    <div class="p-3">
                        <h3 class="text-sm font-medium">Valorant</h3>
                        <p class="text-xs text-gray-500">Last played: Today</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden cursor-pointer">
                    <div class="h-24 bg-gray-200 overflow-hidden">
                        <img src="https://readdy.ai/api/search-image?query=minecraft%20game%20screenshot%2C%20building%20blocks%2C%20creative%20mode%2C%20landscape%20view%2C%20colorful%20world&width=160&height=120&seq=4&orientation=landscape" alt="Minecraft" class="w-full h-full object-cover object-top">
                    </div>
                    <div class="p-3">
                        <h3 class="text-sm font-medium">Minecraft</h3>
                        <p class="text-xs text-gray-500">Last played: Yesterday</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden cursor-pointer">
                    <div class="h-24 bg-gray-200 overflow-hidden">
                        <img src="https://readdy.ai/api/search-image?query=fortnite%20game%20screenshot%2C%20battle%20royale%2C%20colorful%20environment%2C%20action%20scene%2C%20no%20faces%20visible&width=160&height=120&seq=5&orientation=landscape" alt="Fortnite" class="w-full h-full object-cover object-top">
                    </div>
                    <div class="p-3">
                        <h3 class="text-sm font-medium">Fortnite</h3>
                        <p class="text-xs text-gray-500">Last played: 2 days ago</p>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm overflow-hidden cursor-pointer">
                    <div class="h-24 bg-gray-200 overflow-hidden">
                        <img src="https://readdy.ai/api/search-image?query=league%20of%20legends%20game%20screenshot%2C%20moba%20gameplay%2C%20fantasy%20characters%2C%20battle%20scene%2C%20vibrant%20colors&width=160&height=120&seq=6&orientation=landscape" alt="League of Legends" class="w-full h-full object-cover object-top">
                    </div>
                    <div class="p-3">
                        <h3 class="text-sm font-medium">League of Legends</h3>
                        <p class="text-xs text-gray-500">Last played: 3 days ago</p>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- My Music Library -->
        <section>
            <div class="flex justify-between items-center mb-4">
                <h2 class="text-lg font-semibold">My Music Library</h2>
                <button class="text-sm text-primary cursor-pointer">View All</button>
            </div>
            
            <div class="space-y-2">
                <div class="flex items-center p-3 bg-white rounded-lg shadow-sm cursor-pointer">
                    <div class="w-10 h-10 rounded bg-gray-200 overflow-hidden mr-3">
                        <img src="https://readdy.ai/api/search-image?query=abstract%20album%20art%2C%20blue%20theme%2C%20minimalist%20design%2C%20electronic%20music&width=80&height=80&seq=7&orientation=squarish" alt="Album Cover" class="w-full h-full object-cover">
                    </div>
                    <div class="flex-1">
                        <p class="text-sm font-medium">Save Your Tears</p>
                        <p class="text-xs text-gray-500">The Weeknd</p>
                    </div>
                    <div class="w-8 h-8 flex items-center justify-center">
                        <i class="ri-play-circle-line text-primary ri-lg"></i>
                    </div>
                </div>
                
                <div class="flex items-center p-3 bg-white rounded-lg shadow-sm cursor-pointer">
                    <div class="w-10 h-10 rounded bg-gray-200 overflow-hidden mr-3">
                        <img src="https://readdy.ai/api/search-image?query=abstract%20album%20art%2C%20red%20and%20black%20theme%2C%20rock%20music%2C%20edgy%20design&width=80&height=80&seq=8&orientation=squarish" alt="Album Cover" class="w-full h-full object-cover">
                    </div>
                    <div class="flex-1">
                        <p class="text-sm font-medium">Heathens</p>
                        <p class="text-xs text-gray-500">Twenty One Pilots</p>
                    </div>
                    <div class="w-8 h-8 flex items-center justify-center">
                        <i class="ri-play-circle-line text-primary ri-lg"></i>
                    </div>
                </div>
                
                <div class="flex items-center p-3 bg-white rounded-lg shadow-sm cursor-pointer">
                    <div class="w-10 h-10 rounded bg-gray-200 overflow-hidden mr-3">
                        <img src="https://readdy.ai/api/search-image?query=abstract%20album%20art%2C%20purple%20theme%2C%20pop%20music%2C%20vibrant%20design&width=80&height=80&seq=9&orientation=squarish" alt="Album Cover" class="w-full h-full object-cover">
                    </div>
                    <div class="flex-1">
                        <p class="text-sm font-medium">As It Was</p>
                        <p class="text-xs text-gray-500">Harry Styles</p>
                    </div>
                    <div class="w-8 h-8 flex items-center justify-center">
                        <i class="ri-play-circle-line text-primary ri-lg"></i>
                    </div>
                </div>
                
                <div class="flex items-center p-3 bg-white rounded-lg shadow-sm cursor-pointer">
                    <div class="w-10 h-10 rounded bg-gray-200 overflow-hidden mr-3">
                        <img src="https://readdy.ai/api/search-image?query=abstract%20album%20art%2C%20green%20theme%2C%20indie%20music%2C%20artistic%20design&width=80&height=80&seq=10&orientation=squarish" alt="Album Cover" class="w-full h-full object-cover">
                    </div>
                    <div class="flex-1">
                        <p class="text-sm font-medium">Chlorine</p>
                        <p class="text-xs text-gray-500">Twenty One Pilots</p>
                    </div>
                    <div class="w-8 h-8 flex items-center justify-center">
                        <i class="ri-play-circle-line text-primary ri-lg"></i>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Floating Action Button -->
    <button class="fixed right-4 bottom-20 w-14 h-14 bg-primary rounded-full shadow-lg flex items-center justify-center cursor-pointer !rounded-button">
        <i class="ri-add-line text-white ri-2x"></i>
    </button>

    <!-- Tab bar -->
    <nav class="fixed bottom-0 w-full bg-white border-t border-gray-200 z-50">
        <div class="grid grid-cols-4 h-16">
            <button class="flex flex-col items-center justify-center cursor-pointer">
                <div class="w-6 h-6 flex items-center justify-center">
                    <i class="ri-home-4-line text-primary ri-lg"></i>
                </div>
                <span class="text-xs mt-1 text-primary">Home</span>
            </button>
            
            <button class="flex flex-col items-center justify-center cursor-pointer">
                <div class="w-6 h-6 flex items-center justify-center">
                    <i class="ri-music-2-line text-gray-500 ri-lg"></i>
                </div>
                <span class="text-xs mt-1 text-gray-500">Music</span>
            </button>
            
            <button class="flex flex-col items-center justify-center cursor-pointer">
                <div class="w-6 h-6 flex items-center justify-center">
                    <i class="ri-gamepad-line text-gray-500 ri-lg"></i>
                </div>
                <span class="text-xs mt-1 text-gray-500">Games</span>
            </button>
            
            <button class="flex flex-col items-center justify-center cursor-pointer">
                <div class="w-6 h-6 flex items-center justify-center">
                    <i class="ri-user-settings-line text-gray-500 ri-lg"></i>
                </div>
                <span class="text-xs mt-1 text-gray-500">Profile</span>
            </button>
        </div>
    </nav>

    <!-- New Post Modal (Hidden by default) -->
    <div id="newPostModal" class="fixed inset-0 bg-black bg-opacity-50 z-50 flex items-center justify-center hidden">
        <div class="bg-white rounded-lg w-[90%] max-w-md">
            <div class="p-4 border-b border-gray-200">
                <h3 class="text-lg font-medium">Create New Post</h3>
            </div>
            <div class="p-4">
                <textarea class="w-full border border-gray-200 rounded-lg p-3 text-sm h-32 focus:outline-none focus:border-primary" placeholder="What's on your mind?"></textarea>
                <div class="flex items-center space-x-3 mt-3">
                    <button class="w-8 h-8 flex items-center justify-center rounded-full bg-gray-100 cursor-pointer">
                        <i class="ri-image-line text-gray-600"></i>
                    </button>
                    <button class="w-8 h-8 flex items-center justify-center rounded-full bg-gray-100 cursor-pointer">
                        <i class="ri-emotion-line text-gray-60
