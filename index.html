<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>iOS 全屏模拟</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+SC:wght@400;500;700&family=SF+Pro+Display:wght@400;500;600;700&display=swap" rel="stylesheet">

    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", "Noto Sans SC", sans-serif;
            background-color: #e5e0da;
            user-select: none;
            -webkit-user-select: none;
        }

        .no-scrollbar::-webkit-scrollbar {
            display: none;
        }
        .no-scrollbar {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        .ios-wallpaper {
            background: linear-gradient(160deg, #F3ECE1 0%, #E8D8CE 40%, #D8DFE5 100%);
        }

        .app-view {
            transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .app-view.hidden-app {
            opacity: 0;
            transform: scale(0.95);
            pointer-events: none;
        }
        .app-view.active-app {
            opacity: 1;
            transform: scale(1);
            pointer-events: auto;
        }

        .soft-shadow {
            box-shadow: 0 4px 20px -2px rgba(175, 165, 150, 0.15);
        }

        .modal-overlay {
            transition: opacity 0.25s ease, visibility 0.25s ease;
        }
        .modal-sheet {
            transition: transform 0.35s cubic-bezier(0.32, 0.72, 0, 1);
        }
        .modal-sheet.slide-up {
            transform: translateY(0);
        }
        .modal-sheet.slide-down {
            transform: translateY(100%);
        }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center m-0 p-0 overflow-hidden">

    <!-- 全屏设备容器 (已取消顶部时间状态栏) -->
    <main class="w-screen h-screen bg-white relative overflow-hidden flex flex-col shadow-2xl">

        <!-- 应用主容器 -->
        <div id="screen-container" class="relative w-full h-full pb-5 overflow-hidden flex flex-col">

            <!-- ================= 主屏幕 (HOME) ================= -->
            <div id="app-home" class="w-full h-full ios-wallpaper p-5 pt-8 flex flex-col justify-between">
                <div>
                    <div class="bg-white/75 backdrop-blur-md rounded-3xl p-4 soft-shadow border border-white/60">
                        <div class="text-xs font-semibold text-stone-400 uppercase tracking-wider" id="widget-date">7月29日 周三</div>
                        <div class="text-2xl font-bold text-stone-800 mt-1" id="widget-greeting">祝您度过美好的一天 🌸</div>
                        <div class="mt-3 flex items-center justify-between text-xs text-stone-600 bg-white/60 px-3 py-1.5 rounded-xl border border-white/40">
                            <span class="flex items-center gap-1.5"><i class="fa-solid fa-sun text-amber-400"></i> Tokyo 24°C</span>
                            <span class="text-stone-400">晴朗</span>
                        </div>
                    </div>
                </div>

                <div class="grid grid-cols-4 gap-y-6 gap-x-4 px-2 my-auto">
                    <!-- LINE -->
                    <button onclick="openApp('line')" class="flex flex-col items-center gap-1.5 group">
                        <div class="w-14 h-14 bg-[#06C755] rounded-[18px] flex items-center justify-center text-white text-2xl shadow-lg shadow-emerald-500/20 group-active:scale-95 transition-transform">
                            <i class="fa-comment-dots fa-solid"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700 tracking-tight">LINE</span>
                    </button>

                    <!-- Instagram -->
                    <button onclick="openApp('ins')" class="flex flex-col items-center gap-1.5 group">
                        <div class="w-14 h-14 bg-gradient-to-tr from-amber-400 via-rose-500 to-purple-600 rounded-[18px] flex items-center justify-center text-white text-2xl shadow-lg shadow-rose-500/20 group-active:scale-95 transition-transform">
                            <i class="fa-brands fa-instagram"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700 tracking-tight">Instagram</span>
                    </button>

                    <!-- X (推特) -->
                    <button onclick="openApp('x')" class="flex flex-col items-center gap-1.5 group">
                        <div class="w-14 h-14 bg-stone-900 rounded-[18px] flex items-center justify-center text-white text-2xl shadow-lg shadow-stone-900/20 group-active:scale-95 transition-transform">
                            <i class="fa-brands fa-x-twitter"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700 tracking-tight">X</span>
                    </button>

                    <!-- 通讯录 -->
                    <button onclick="openApp('contacts')" class="flex flex-col items-center gap-1.5 group">
                        <div class="w-14 h-14 bg-stone-300 rounded-[18px] flex items-center justify-center text-stone-700 text-2xl shadow-lg shadow-stone-400/20 group-active:scale-95 transition-transform">
                            <i class="fa-solid fa-address-book"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700 tracking-tight">通讯录</span>
                    </button>

                    <!-- 设置 -->
                    <button onclick="openApp('settings')" class="flex flex-col items-center gap-1.5 group">
                        <div class="w-14 h-14 bg-stone-200/90 backdrop-blur rounded-[18px] flex items-center justify-center text-stone-700 text-2xl shadow-md border border-white/80 group-active:scale-95 transition-transform">
                            <i class="fa-solid fa-gear"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700 tracking-tight">设置</span>
                    </button>

                    <div class="flex flex-col items-center gap-1.5 opacity-60">
                        <div class="w-14 h-14 bg-sky-400 rounded-[18px] flex items-center justify-center text-white text-2xl shadow-md">
                            <i class="fa-regular fa-clock"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700">时钟</span>
                    </div>
                    <div class="flex flex-col items-center gap-1.5 opacity-60">
                        <div class="w-14 h-14 bg-amber-400 rounded-[18px] flex items-center justify-center text-white text-2xl shadow-md">
                            <i class="fa-solid fa-images"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700">相册</span>
                    </div>
                    <div class="flex flex-col items-center gap-1.5 opacity-60">
                        <div class="w-14 h-14 bg-rose-400 rounded-[18px] flex items-center justify-center text-white text-2xl shadow-md">
                            <i class="fa-solid fa-music"></i>
                        </div>
                        <span class="text-[11px] font-medium text-stone-700">音乐</span>
                    </div>
                </div>

                <div class="bg-white/40 backdrop-blur-xl rounded-[28px] p-2.5 flex justify-around items-center border border-white/50 shadow-sm mb-2">
                    <div class="w-12 h-12 bg-emerald-500 rounded-[16px] flex items-center justify-center text-white text-xl shadow-md">
                        <i class="fa-solid fa-phone"></i>
                    </div>
                    <div class="w-12 h-12 bg-sky-500 rounded-[16px] flex items-center justify-center text-white text-xl shadow-md">
                        <i class="fa-solid fa-compass"></i>
                    </div>
                    <div class="w-12 h-12 bg-emerald-600 rounded-[16px] flex items-center justify-center text-white text-xl shadow-md">
                        <i class="fa-solid fa-message"></i>
                    </div>
                    <div class="w-12 h-12 bg-rose-500 rounded-[16px] flex items-center justify-center text-white text-xl shadow-md">
                        <i class="fa-solid fa-heart"></i>
                    </div>
                </div>
            </div>

            <!-- ================= 通讯录 App ================= -->
            <div id="app-contacts" class="app-view hidden-app absolute inset-0 bg-stone-50 z-20 flex flex-col pt-4">
                <div class="bg-white/90 backdrop-blur px-4 py-3 border-b border-stone-200/60 sticky top-0 z-10 flex items-center justify-between">
                    <h2 class="text-base font-bold text-stone-800">通讯录</h2>
                    <button onclick="openCreateCharacterModal()" class="text-sky-500 hover:text-sky-600 p-1 text-lg active:scale-95 transition-transform">
                        <i class="fa-solid fa-plus"></i>
                    </button>
                </div>

                <div class="flex-1 overflow-y-auto p-4 space-y-3 no-scrollbar" id="contacts-list"></div>

                <!-- 新建 / 编辑角色弹窗 -->
                <div id="modal-create-character" class="modal-overlay absolute inset-0 bg-black/40 z-50 flex flex-col justify-end opacity-0 pointer-events-none">
                    <div id="modal-create-sheet" class="modal-sheet slide-down w-full h-[95%] bg-white rounded-t-2xl flex flex-col pt-3 px-5 pb-6 shadow-2xl">
                        <div class="flex items-center justify-between py-2 mb-2 border-b border-stone-100">
                            <span class="text-xs font-semibold text-stone-400 cursor-pointer" onclick="closeCreateCharacterModal()">取消</span>
                            <h2 class="text-base font-bold text-black" id="modal-character-title">新建联系人</h2>
                            <button onclick="manualSaveCharacter()" class="text-xs font-bold text-emerald-500">保存</button>
                        </div>

                        <div class="flex-1 overflow-y-auto pt-2 space-y-4 no-scrollbar">
                            <div class="flex items-center gap-4 bg-stone-50 p-3 rounded-2xl border border-stone-200/60">
                                <img id="preview-avatar" src="https://via.placeholder.com/60/07c160/ffffff?text=AI" class="w-14 h-14 rounded-2xl object-cover border border-stone-200">
                                <div>
                                    <button onclick="document.getElementById('avatar-input').click()" class="bg-white border border-stone-300 px-3 py-1.5 rounded-xl text-xs font-semibold text-stone-700 active:scale-95 transition-transform">
                                        上传头像
                                    </button>
                                    <input type="file" id="avatar-input" accept="image/*" class="hidden" onchange="handleAvatarUpload(event)">
                                </div>
                            </div>

                            <div class="bg-stone-50 rounded-2xl border border-stone-200/60 p-3.5 space-y-3">
                                <div>
                                    <label class="block text-stone-500 text-[11px] font-bold mb-1">姓名 <span class="text-rose-500">*</span></label>
                                    <input type="text" id="input-name" placeholder="请输入角色姓名" class="w-full bg-white border border-stone-200 rounded-xl p-2.5 text-xs text-stone-800 focus:outline-none focus:ring-1 focus:ring-sky-400">
                                </div>
                                <div>
                                    <label class="block text-stone-500 text-[11px] font-bold mb-1">备注</label>
                                    <input type="text" id="input-alias" placeholder="请输入备注名（可选）" class="w-full bg-white border border-stone-200 rounded-xl p-2.5 text-xs text-stone-800 focus:outline-none focus:ring-1 focus:ring-sky-400">
                                </div>
                                <div>
                                    <label class="block text-stone-500 text-[11px] font-bold mb-1">LINE ID</label>
                                    <div class="flex gap-2">
                                        <input type="text" id="input-line-id" placeholder="可自定义或点右侧自动生成" class="flex-1 bg-white border border-stone-200 rounded-xl p-2.5 text-xs text-stone-800 focus:outline-none focus:ring-1 focus:ring-sky-400">
                                        <button onclick="generateRandomID()" class="bg-stone-200 text-stone-700 font-semibold px-3 py-2 rounded-xl text-xs whitespace-nowrap active:scale-95 transition-transform">
                                            自动生成 ID
                                        </button>
                                    </div>
                                </div>
                                <div>
                                    <label class="block text-stone-500 text-[11px] font-bold mb-1">手机号码</label>
                                    <input type="text" id="input-phone" placeholder="11位手机号（可选）" class="w-full bg-white border border-stone-200 rounded-xl p-2.5 text-xs text-stone-800 focus:outline-none focus:ring-1 focus:ring-sky-400">
                                </div>
                            </div>

                            <div class="bg-stone-50 rounded-2xl border border-stone-200/60 p-3.5">
                                <label class="block text-stone-800 text-xs font-bold mb-1.5">人设 / 性格设定</label>
                                <textarea id="persona-input" rows="4" placeholder="例如：傲娇的二次元黑客少女，喜欢喝草莓牛奶..." class="w-full bg-white border border-stone-200 rounded-xl p-2.5 text-xs text-stone-700 focus:outline-none focus:ring-1 focus:ring-sky-400"></textarea>
                                
                                <div class="mt-3 pt-3 border-t border-stone-200/60 flex items-center justify-between">
                                    <span class="text-[10px] text-stone-400">也可以输入提示词由 AI 填充：</span>
                                    <button onclick="generateCharacter()" id="generate-btn" class="bg-sky-500 text-white font-bold px-3 py-1.5 rounded-xl active:scale-95 transition-transform text-xs">
                                        通过 API 生成
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ================= LINE App ================= -->
            <div id="app-line" class="app-view hidden-app absolute inset-0 bg-white z-20 flex flex-col pt-4">
                
                <!-- Tab 1: 主页视图 -->
                <div id="line-tab-view-home" class="flex-1 overflow-y-auto no-scrollbar px-4 pt-2 pb-16">
                    <div class="flex justify-end items-center gap-4 text-stone-800 text-lg py-2">
                        <i class="fa-regular fa-bookmark"></i>
                        <i class="fa-regular fa-bell"></i>
                        <i class="fa-solid fa-user-plus cursor-pointer" onclick="openLineAddModal()"></i>
                        <i class="fa-solid fa-gear cursor-pointer" onclick="openApp('settings')"></i>
                    </div>

                    <div class="flex justify-between items-center my-3">
                        <div>
                            <h1 class="text-2xl font-extrabold text-black tracking-tight">wenj</h1>
                            <p class="text-xs text-stone-400 mt-1">输入状态消息</p>
                        </div>
                        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=120&auto=format&fit=crop&q=80" class="w-14 h-14 rounded-full object-cover border border-stone-100 shadow-sm">
                    </div>

                    <div class="relative my-4">
                        <div class="w-full bg-[#F5F5F5] rounded-full flex items-center px-4 py-2 text-stone-400">
                            <i class="fa-solid fa-magnifying-glass text-stone-400 text-sm mr-2"></i>
                            <input type="text" placeholder="搜索" class="bg-transparent text-xs text-stone-800 w-full focus:outline-none placeholder-stone-400">
                            <i class="fa-solid fa-expand text-stone-600 text-sm ml-2"></i>
                        </div>
                    </div>

                    <div class="mt-5">
                        <div class="flex justify-between items-center mb-3">
                            <span class="text-sm font-bold text-black">服务</span>
                            <span class="text-xs text-stone-400 font-medium cursor-pointer">显示全部</span>
                        </div>
                        <div class="grid grid-cols-4 text-center py-1">
                            <div class="flex flex-col items-center gap-1.5 cursor-pointer">
                                <div class="w-10 h-10 rounded-full flex items-center justify-center text-xl text-black"><i class="fa-regular fa-face-smile"></i></div>
                                <span class="text-[11px] font-medium text-stone-700">贴图</span>
                            </div>
                            <div class="flex flex-col items-center gap-1.5 cursor-pointer">
                                <div class="w-10 h-10 rounded-full flex items-center justify-center text-xl text-black"><i class="fa-solid fa-stamp"></i></div>
                                <span class="text-[11px] font-medium text-stone-700">主题</span>
                            </div>
                            <div class="flex flex-col items-center gap-1.5 cursor-pointer">
                                <div class="w-10 h-10 rounded-full flex items-center justify-center text-xl text-black"><i class="fa-regular fa-shield"></i></div>
                                <span class="text-[11px] font-medium text-stone-700">官方账号</span>
                            </div>
                            <div class="flex flex-col items-center gap-1.5 cursor-pointer">
                                <div class="w-10 h-10 rounded-full flex items-center justify-center text-xl text-black"><i class="fa-solid fa-gamepad"></i></div>
                                <span class="text-[11px] font-medium text-stone-700">LINE GAME</span>
                            </div>
                        </div>
                    </div>

                    <div class="mt-6 space-y-4">
                        <div class="flex justify-between items-center cursor-pointer">
                            <span class="text-sm font-bold text-black">群</span>
                            <i class="fa-solid fa-chevron-down text-xs text-stone-400"></i>
                        </div>
                        <div>
                            <div class="flex justify-between items-center cursor-pointer mb-3">
                                <span class="text-sm font-bold text-black">好友</span>
                                <i class="fa-solid fa-chevron-up text-xs text-stone-400"></i>
                            </div>
                            <div id="line-friends-list" class="space-y-1">
                                <div class="text-xs text-stone-400 py-2">暂无好友</div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Tab 2: 聊天列表视图 -->
                <div id="line-tab-view-chats" class="flex-1 overflow-y-auto no-scrollbar px-4 pt-2 pb-16 hidden">
                    <div class="flex justify-between items-center py-2 mb-2">
                        <h1 class="text-2xl font-extrabold text-black tracking-tight">聊天</h1>
                        <div class="flex gap-4 text-stone-800 text-lg">
                            <i class="fa-regular fa-comment-dots"></i>
                            <i class="fa-solid fa-list-check"></i>
                        </div>
                    </div>
                    <div id="line-chat-threads-list" class="divide-y divide-stone-100">
                        <div class="text-center text-xs text-stone-400 py-12">暂无聊天，在搜索中添加好友吧！</div>
                    </div>
                </div>

                <!-- Tab 3: 通话视图 -->
                <div id="line-tab-view-calls" class="flex-1 flex items-center justify-center text-xs text-stone-400 hidden">
                    暂无通话记录
                </div>

                <!-- 聊天详情界面 -->
                <div id="line-chat-detail-view" class="absolute inset-0 bg-[#8cabd9] z-40 flex flex-col hidden">
                    <div class="bg-[#8cabd9]/90 backdrop-blur px-4 py-2 border-b border-white/20 flex items-center justify-between text-white">
                        <div class="flex items-center gap-3">
                            <i class="fa-solid fa-chevron-left text-lg cursor-pointer" onclick="closeChatDetail()"></i>
                            <span id="chat-title-name" class="font-bold text-sm">好友姓名</span>
                        </div>
                        <div class="flex items-center gap-4 text-base">
                            <i class="fa-solid fa-magnifying-glass"></i>
                            <i class="fa-solid fa-phone"></i>
                            <i class="fa-solid fa-bars"></i>
                        </div>
                    </div>

                    <div id="chat-messages-container" class="flex-1 p-4 overflow-y-auto no-scrollbar space-y-3">
                        <div class="text-center text-[10px] text-white/70 my-2">我们已经是好友了，现在可以开始聊天了</div>
                    </div>

                    <div class="bg-white px-3 py-2 flex items-center gap-2 border-t border-stone-200">
                        <i class="fa-solid fa-plus text-stone-500 text-lg"></i>
                        <i class="fa-solid fa-camera text-stone-500 text-lg"></i>
                        <i class="fa-regular fa-image text-stone-500 text-lg"></i>
                        <input type="text" id="chat-input-field" placeholder="发送消息" class="flex-1 bg-stone-100 rounded-full px-3 py-1.5 text-xs text-stone-800 focus:outline-none">
                        <i class="fa-regular fa-face-smile text-stone-500 text-lg"></i>
                    </div>
                </div>

                <!-- LINE 底部导航 -->
                <div class="absolute bottom-0 left-0 w-full bg-white border-t border-stone-100 py-2 px-8 flex justify-around items-center z-30">
                    <button onclick="switchLineTab('home')" id="tab-btn-home" class="flex flex-col items-center gap-0.5 text-black">
                        <i class="fa-solid fa-house text-lg"></i>
                        <span class="text-[10px] font-bold">主页</span>
                    </button>
                    <button onclick="switchLineTab('chats')" id="tab-btn-chats" class="flex flex-col items-center gap-0.5 text-stone-400 hover:text-black transition-colors">
                        <i class="fa-regular fa-comment-dots text-lg"></i>
                        <span class="text-[10px] font-medium">聊天</span>
                    </button>
                    <button onclick="switchLineTab('calls')" id="tab-btn-calls" class="flex flex-col items-center gap-0.5 text-stone-400 hover:text-black transition-colors">
                        <i class="fa-solid fa-phone text-lg"></i>
                        <span class="text-[10px] font-medium">通话</span>
                    </button>
                </div>

                <!-- LINE 添加好友抽屉 -->
                <div id="modal-line-add-friends" class="modal-overlay absolute inset-0 bg-black/40 z-40 flex flex-col justify-end opacity-0 pointer-events-none">
                    <div id="modal-sheet-content" class="modal-sheet slide-down w-full h-[93%] bg-white rounded-t-2xl flex flex-col pt-3 px-5 pb-6 shadow-2xl">
                        <div class="flex items-center justify-between py-2 mb-2">
                            <i class="fa-solid fa-gear text-stone-800 text-lg cursor-pointer" onclick="openApp('settings')"></i>
                            <h2 class="text-base font-bold text-black">添加好友</h2>
                            <i class="fa-solid fa-xmark text-stone-800 text-2xl cursor-pointer" onclick="closeAllLineModals()"></i>
                        </div>
                        <div class="grid grid-cols-3 py-6 border-b border-stone-100 text-center">
                            <div class="flex flex-col items-center gap-2 cursor-pointer group">
                                <i class="fa-solid fa-plus text-3xl text-stone-800 font-light group-active:scale-90 transition-transform"></i>
                                <span class="text-xs text-stone-600 font-medium">邀请</span>
                            </div>
                            <div class="flex flex-col items-center gap-2 cursor-pointer group">
                                <i class="fa-solid fa-qrcode text-3xl text-stone-800 group-active:scale-90 transition-transform"></i>
                                <span class="text-xs text-stone-600 font-medium">二维码</span>
                            </div>
                            <div onclick="openLineSearchModal()" class="flex flex-col items-center gap-2 cursor-pointer group">
                                <i class="fa-solid fa-magnifying-glass text-3xl text-stone-800 group-active:scale-90 transition-transform"></i>
                                <span class="text-xs text-stone-600 font-medium">搜索</span>
                            </div>
                        </div>
                        <div class="py-5 space-y-6">
                            <div class="flex items-center justify-between">
                                <div class="flex items-center gap-3.5">
                                    <div class="w-10 h-10 rounded-full bg-[#06C755] flex items-center justify-center text-white text-lg shadow-sm"><i class="fa-solid fa-user-plus"></i></div>
                                    <div>
                                        <h3 class="text-sm font-bold text-black">自动添加好友</h3>
                                        <p class="text-[11px] text-stone-400 mt-0.5">将联系人自动添加为好友。</p>
                                    </div>
                                </div>
                                <button class="bg-[#06C755] text-white text-xs font-semibold px-4 py-1.5 rounded-lg active:opacity-80 transition-opacity">允许</button>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- LINE 搜索好友抽屉 -->
                <div id="modal-line-search-friends" class="modal-overlay absolute inset-0 bg-black/40 z-50 flex flex-col justify-end opacity-0 pointer-events-none">
                    <div id="modal-search-sheet-content" class="modal-sheet slide-down w-full h-[93%] bg-white rounded-t-2xl flex flex-col pt-3 px-5 pb-6 shadow-2xl">
                        <div class="flex items-center justify-between py-2 mb-4">
                            <i class="fa-solid fa-chevron-left text-stone-800 text-lg cursor-pointer" onclick="backToAddFriendsModal()"></i>
                            <h2 class="text-base font-bold text-black">搜索好友</h2>
                            <i class="fa-solid fa-xmark text-stone-800 text-2xl cursor-pointer" onclick="closeAllLineModals()"></i>
                        </div>
                        <div class="flex items-center gap-8 py-2 mb-5">
                            <label class="flex items-center gap-2 cursor-pointer group" onclick="setSearchType('id')">
                                <div id="radio-id-outer" class="w-4 h-4 rounded-full border-2 border-[#06C755] flex items-center justify-center p-0.5">
                                    <div id="radio-id-inner" class="w-full h-full rounded-full bg-[#06C755]"></div>
                                </div>
                                <span class="text-xs font-semibold text-black">ID</span>
                            </label>
                            <label class="flex items-center gap-2 cursor-pointer group" onclick="setSearchType('phone')">
                                <div id="radio-phone-outer" class="w-4 h-4 rounded-full border border-stone-300 flex items-center justify-center p-0.5">
                                    <div id="radio-phone-inner" class="w-full h-full rounded-full bg-transparent"></div>
                                </div>
                                <span class="text-xs font-semibold text-black">电话号码</span>
                            </label>
                        </div>
                        <div class="relative">
                            <input type="text" id="line-search-input" placeholder="输入好友的 ID" class="w-full bg-[#F5F5F5] rounded-lg py-2.5 pl-3 pr-10 text-xs text-stone-800 focus:outline-none placeholder-stone-400">
                            <i class="fa-solid fa-magnifying-glass absolute right-3 top-1/2 -translate-y-1/2 text-stone-300 text-sm cursor-pointer" onclick="searchLineFriend(document.getElementById('line-search-input').value.trim())"></i>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ================= Instagram App ================= -->
            <div id="app-ins" class="app-view hidden-app absolute inset-0 bg-white z-20 flex flex-col pt-4">
                <div class="bg-white border-b border-stone-100 px-4 py-2 flex items-center justify-between sticky top-0 z-10">
                    <span class="font-serif italic font-bold text-xl tracking-tight text-stone-900">Instagram</span>
                    <div class="flex items-center gap-4 text-lg text-stone-800">
                        <i class="fa-regular fa-heart"></i>
                        <i class="fa-regular fa-paper-plane"></i>
                    </div>
                </div>
                <div class="flex-1 overflow-y-auto no-scrollbar">
                    <div class="flex gap-3 px-4 py-3 border-b border-stone-100 overflow-x-auto no-scrollbar">
                        <div class="flex flex-col items-center gap-1 flex-shrink-0">
                            <div class="p-0.5 rounded-full border border-stone-200"><img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=100&auto=format&fit=crop&q=80" class="w-11 h-11 rounded-full object-cover"></div>
                            <span class="text-[10px] text-stone-500">限时动态</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ================= X App ================= -->
            <div id="app-x" class="app-view hidden-app absolute inset-0 bg-white z-20 flex flex-col pt-4">
                <div class="bg-white border-b border-stone-100 sticky top-0 z-10">
                    <div class="flex justify-between items-center px-4 py-2">
                        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=100&auto=format&fit=crop&q=80" class="w-7 h-7 rounded-full object-cover">
                        <i class="fa-brands fa-x-twitter text-lg text-stone-900"></i>
                        <i class="fa-solid fa-gear text-stone-600 text-xs"></i>
                    </div>
                </div>
            </div>

            <!-- ================= 设置 App ================= -->
            <div id="app-settings" class="app-view hidden-app absolute inset-0 bg-stone-100 z-20 flex flex-col pt-4">
                <div class="bg-white/90 backdrop-blur px-4 py-3 border-b border-stone-200/60 sticky top-0 z-10 flex items-center justify-between">
                    <h2 class="text-base font-bold text-stone-800">设置</h2>
                    <button onclick="goHome()" class="text-xs font-semibold text-rose-500">完成</button>
                </div>

                <div class="flex-1 overflow-y-auto p-4 space-y-4 text-xs no-scrollbar">
                    <div>
                        <div class="text-stone-400 px-2 mb-1.5 uppercase tracking-wider text-[10px] font-semibold">语言 / LANGUAGE</div>
                        <div class="bg-white rounded-2xl border border-stone-200/60 overflow-hidden divide-y divide-stone-100">
                            <label class="flex items-center justify-between p-3 cursor-pointer hover:bg-stone-50">
                                <span class="font-medium text-stone-700">简体中文</span>
                                <input type="radio" name="lang" value="zh" checked class="accent-rose-500">
                            </label>
                        </div>
                    </div>

                    <div>
                        <div class="text-stone-400 px-2 mb-1.5 uppercase tracking-wider text-[10px] font-semibold">API 连接设置</div>
                        <div class="bg-white rounded-2xl border border-stone-200/60 p-3 space-y-3">
                            <div>
                                <label class="block text-stone-500 mb-1 font-medium">Base URL</label>
                                <input type="text" id="api-url" placeholder="https://api.openai.com/v1" class="w-full bg-stone-50 border border-stone-200 rounded-xl p-2 text-stone-700 focus:outline-none focus:ring-1 focus:ring-rose-400">
                            </div>
                            <div>
                                <label class="block text-stone-500 mb-1 font-medium">API Key</label>
                                <input type="password" id="api-key" placeholder="sk-..." class="w-full bg-stone-50 border border-stone-200 rounded-xl p-2 text-stone-700 focus:outline-none focus:ring-1 focus:ring-rose-400">
                            </div>
                            <div>
                                <label class="block text-stone-500 mb-1 font-medium">Model Name</label>
                                <input type="text" id="api-model" placeholder="gpt-4o" class="w-full bg-stone-50 border border-stone-200 rounded-xl p-2 text-stone-700 focus:outline-none focus:ring-1 focus:ring-rose-400">
                            </div>
                            <button onclick="saveApiConfig()" class="w-full bg-stone-800 text-white font-medium py-2 rounded-xl active:scale-98 transition-transform">
                                保存设置
                            </button>
                        </div>
                    </div>
                </div>
            </div>

        </div>

        <!-- iOS 底部 Home Indicator Bar -->
        <button onclick="goHome()" class="w-full bg-transparent py-2 flex justify-center items-center absolute bottom-0 left-0 z-50 cursor-pointer active:opacity-60">
            <div class="w-32 h-1 bg-stone-400/80 hover:bg-stone-600 rounded-full transition-colors"></div>
        </button>

    </main>

    <!-- JS 逻辑控制 -->
    <script>
        const DEFAULT_AVATAR = "https://via.placeholder.com/60/07c160/ffffff?text=AI";
        let currentAvatarData = DEFAULT_AVATAR;
        let createdCharactersList = [];
        let addedLineFriends = []; 
        let editingCharacterId = null; // 当前正在编辑的角色 ID（为 null 表示新建）
        let currentSearchType = 'id';

        function resetCreateCharacterForm() {
            editingCharacterId = null;
            document.getElementById('modal-character-title').innerText = "新建联系人";
            document.getElementById('input-name').value = '';
            document.getElementById('input-alias').value = '';
            document.getElementById('input-line-id').value = '';
            document.getElementById('input-phone').value = '';
            document.getElementById('persona-input').value = '';
            currentAvatarData = DEFAULT_AVATAR;
            document.getElementById('preview-avatar').src = DEFAULT_AVATAR;
            document.getElementById('avatar-input').value = '';
        }

        // 打开编辑角色弹窗并载入现有数据
        function openEditCharacterModal(charId) {
            const char = createdCharactersList.find(c => c.id === charId);
            if (!char) return;

            editingCharacterId = char.id;
            document.getElementById('modal-character-title').innerText = "修改联系人 / 人设";
            document.getElementById('input-name').value = char.name || '';
            document.getElementById('input-alias').value = char.alias || '';
            document.getElementById('input-line-id').value = char.line_id || '';
            document.getElementById('input-phone').value = char.phone || '';
            document.getElementById('persona-input').value = char.persona || '';
            currentAvatarData = char.avatar || DEFAULT_AVATAR;
            document.getElementById('preview-avatar').src = currentAvatarData;

            const modal = document.getElementById('modal-create-character');
            const sheet = document.getElementById('modal-create-sheet');
            modal.classList.remove('pointer-events-none', 'opacity-0');
            modal.classList.add('opacity-100');
            sheet.classList.remove('slide-down');
            sheet.classList.add('slide-up');
        }

        function generateRandomID() {
            const randomID = 'line_' + Math.random().toString(36).substr(2, 8);
            document.getElementById('input-line-id').value = randomID;
        }

        function handleAvatarUpload(event) {
            const file = event.target.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(evt) {
                    currentAvatarData = evt.target.result;
                    document.getElementById('preview-avatar').src = currentAvatarData;
                };
                reader.readAsDataURL(file);
            }
        }

        function openCreateCharacterModal() {
            resetCreateCharacterForm();
            const modal = document.getElementById('modal-create-character');
            const sheet = document.getElementById('modal-create-sheet');
            modal.classList.remove('pointer-events-none', 'opacity-0');
            modal.classList.add('opacity-100');
            sheet.classList.remove('slide-down');
            sheet.classList.add('slide-up');
        }

        function closeCreateCharacterModal() {
            const modal = document.getElementById('modal-create-character');
            const sheet = document.getElementById('modal-create-sheet');
            sheet.classList.remove('slide-up');
            sheet.classList.add('slide-down');
            modal.classList.remove('opacity-100');
            modal.classList.add('opacity-0', 'pointer-events-none');
        }

        // 保存/修改角色信息
        function manualSaveCharacter() {
            const name = document.getElementById('input-name').value.trim();
            const alias = document.getElementById('input-alias').value.trim();
            const line_id = document.getElementById('input-line-id').value.trim();
            const phone = document.getElementById('input-phone').value.trim();
            const persona = document.getElementById('persona-input').value.trim();

            if (!name) {
                alert("请输入姓名！");
                return;
            }

            if (editingCharacterId) {
                // 编辑修改现有角色
                const index = createdCharactersList.findIndex(c => c.id === editingCharacterId);
                if (index !== -1) {
                    createdCharactersList[index] = {
                        ...createdCharactersList[index],
                        name, alias, line_id, phone, persona,
                        avatar: currentAvatarData
                    };

                    // 同步更新 LINE 已添加的好友数据
                    const lineIndex = addedLineFriends.findIndex(f => f.id === editingCharacterId);
                    if (lineIndex !== -1) {
                        addedLineFriends[lineIndex] = createdCharactersList[index];
                    }
                }
            } else {
                // 新建角色
                const newChar = {
                    id: 'char_' + Date.now(),
                    name: name,
                    alias: alias,
                    line_id: line_id,
                    phone: phone,
                    persona: persona,
                    avatar: currentAvatarData
                };
                createdCharactersList.push(newChar);
            }

            renderContactsList();
            renderLineFriendsAndChats();
            closeCreateCharacterModal();
        }

        // 渲染通讯录列表，赋予卡片点击修改功能
        function renderContactsList() {
            const listContainer = document.getElementById('contacts-list');
            listContainer.innerHTML = '';
            
            if (createdCharactersList.length === 0) {
                listContainer.innerHTML = '<div class="text-center text-stone-400 text-xs py-12">暂无联系人<br>点击右上角 + 添加</div>';
                return;
            }

            createdCharactersList.forEach(char => {
                const displayName = char.alias ? `${char.alias} (${char.name})` : char.name;
                const idText = char.line_id ? `ID: ${char.line_id}` : '未指定 ID';
                const phoneText = char.phone ? ` | 📱 ${char.phone}` : '';

                const item = document.createElement('div');
                item.className = 'bg-white rounded-xl p-3 shadow-sm border border-stone-200/60 flex items-center gap-3 cursor-pointer hover:border-sky-300 active:scale-98 transition-all';
                // 点击卡片直接打开编辑
                item.onclick = () => openEditCharacterModal(char.id);

                item.innerHTML = `
                    <img src="${char.avatar}" class="w-11 h-11 rounded-xl object-cover border border-stone-100 flex-shrink-0">
                    <div class="flex-1 overflow-hidden">
                        <div class="flex justify-between items-center">
                            <span class="font-bold text-stone-800 text-xs truncate">${displayName}</span>
                            <span class="text-[10px] text-sky-500 font-semibold"><i class="fa-solid fa-[#fa-pen]"></i> 修改</span>
                        </div>
                        <div class="text-[10px] text-stone-400 truncate mt-0.5">${idText}${phoneText}</div>
                        <div class="text-[10px] text-stone-500 truncate mt-1">${char.persona ? '人设: ' + char.persona : '暂无人设'}</div>
                    </div>
                `;
                listContainer.appendChild(item);
            });
        }

        // LINE 好友查找
        function searchLineFriend(query) {
            if (!query) return;
            const isIdSearch = currentSearchType === 'id';

            const foundChar = createdCharactersList.find(char => {
                if (isIdSearch) {
                    return char.line_id && (query.toLowerCase() === char.line_id.toLowerCase());
                } else {
                    return char.phone && (query === char.phone);
                }
            });

            if (foundChar) {
                if (!addedLineFriends.some(f => f.id === foundChar.id)) {
                    addedLineFriends.push(foundChar);
                    renderLineFriendsAndChats();
                }
                alert("加好友成功");
                document.getElementById('line-search-input').value = '';
                return;
            }
            alert("未在通讯录中找到该用户，请确认输入的 ID 或手机号与通讯录一致。");
        }

        // 渲染 LINE 的好友和聊天列表
        function renderLineFriendsAndChats() {
            const friendsContainer = document.getElementById('line-friends-list');
            const chatsContainer = document.getElementById('line-chat-threads-list');

            if (addedLineFriends.length === 0) {
                friendsContainer.innerHTML = `<div class="text-xs text-stone-400 py-2">暂无好友</div>`;
                chatsContainer.innerHTML = `<div class="text-center text-xs text-stone-400 py-12">暂无聊天，在搜索中添加好友吧！</div>`;
                return;
            }

            friendsContainer.innerHTML = '';
            chatsContainer.innerHTML = '';

            addedLineFriends.forEach(friend => {
                const displayName = friend.alias || friend.name;

                // 1. 渲染主页好友项
                const friendItem = document.createElement('div');
                friendItem.className = 'flex items-center gap-3 py-2 cursor-pointer hover:bg-stone-50 rounded-xl px-1';
                friendItem.onclick = () => openChatDetail(friend);
                friendItem.innerHTML = `
                    <img src="${friend.avatar}" class="w-10 h-10 rounded-full object-cover border border-stone-100">
                    <span class="text-xs font-bold text-stone-800">${displayName}</span>
                `;
                friendsContainer.appendChild(friendItem);

                // 2. 渲染聊天列表项
                const chatItem = document.createElement('div');
                chatItem.className = 'flex items-center gap-3 py-3 cursor-pointer hover:bg-stone-50 active:bg-stone-100 px-1 border-b border-stone-100';
                chatItem.onclick = () => openChatDetail(friend);
                chatItem.innerHTML = `
                    <img src="${friend.avatar}" class="w-12 h-12 rounded-full object-cover border border-stone-100">
                    <div class="flex-1 overflow-hidden">
                        <div class="flex justify-between items-center mb-1">
                            <span class="text-xs font-bold text-stone-800 truncate">${displayName}</span>
                            <span class="text-[10px] text-stone-400">刚刚</span>
                        </div>
                        <p class="text-[11px] text-stone-400 truncate">点击开始与 ${displayName} 对话...</p>
                    </div>
                `;
                chatsContainer.appendChild(chatItem);
            });
        }

        // 打开聊天界面
        function openChatDetail(friend) {
            closeAllLineModals();
            const displayName = friend.alias || friend.name;
            document.getElementById('chat-title-name').innerText = displayName;
            
            const messagesContainer = document.getElementById('chat-messages-container');
            messagesContainer.innerHTML = `
                <div class="text-center text-[10px] text-white/70 my-2">您已成功添加 ${displayName} 为好友，现在可以开始聊天了</div>
            `;

            document.getElementById('line-chat-detail-view').classList.remove('hidden');
        }

        function closeChatDetail() {
            document.getElementById('line-chat-detail-view').classList.add('hidden');
        }

        function switchLineTab(tabName) {
            document.getElementById('line-tab-view-home').classList.add('hidden');
            document.getElementById('line-tab-view-chats').classList.add('hidden');
            document.getElementById('line-tab-view-calls').classList.add('hidden');

            document.getElementById('tab-btn-home').className = "flex flex-col items-center gap-0.5 text-stone-400 hover:text-black transition-colors";
            document.getElementById('tab-btn-chats').className = "flex flex-col items-center gap-0.5 text-stone-400 hover:text-black transition-colors";
            document.getElementById('tab-btn-calls').className = "flex flex-col items-center gap-0.5 text-stone-400 hover:text-black transition-colors";

            if (tabName === 'home') {
                document.getElementById('line-tab-view-home').classList.remove('hidden');
                document.getElementById('tab-btn-home').className = "flex flex-col items-center gap-0.5 text-black font-bold";
            } else if (tabName === 'chats') {
                document.getElementById('line-tab-view-chats').classList.remove('hidden');
                document.getElementById('tab-btn-chats').className = "flex flex-col items-center gap-0.5 text-black font-bold";
            } else if (tabName === 'calls') {
                document.getElementById('line-tab-view-calls').classList.remove('hidden');
                document.getElementById('tab-btn-calls').className = "flex flex-col items-center gap-0.5 text-black font-bold";
            }
        }

        // AI 填充人设
        async function generateCharacter() {
            const persona = document.getElementById('persona-input').value.trim();
            if (!persona) return alert("请先在文本框中输入角色性格或设定！");

            const apiUrl = localStorage.getItem('api_url');
            const apiKey = localStorage.getItem('api_key');
            const apiModel = localStorage.getItem('api_model') || 'gpt-4o';

            if (!apiUrl || !apiKey) {
                alert("请先在「设置」App 中配置 API URL 和 API Key！");
                closeCreateCharacterModal();
                openApp('settings');
                return;
            }

            const btn = document.getElementById('generate-btn');
            btn.innerText = "生成中...";
            btn.disabled = true;

            try {
                const response = await fetch(`${apiUrl}/chat/completions`, {
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json',
                        'Authorization': `Bearer ${apiKey}`
                    },
                    body: JSON.stringify({
                        model: apiModel,
                        response_format: { type: "json_object" },
                        messages: [
                            { role: "system", content: "你是一个角色生成器。根据用户设定生成 JSON 对象，包含：name(名字), alias(备注名), line_id(8位随机英文+数字), phone(11位随机数字), persona(精简版人设描述，50字内)。" },
                            { role: "user", content: persona }
                        ]
                    })
                });

                const data = await response.json();
                const result = JSON.parse(data.choices[0].message.content);

                document.getElementById('input-name').value = result.name || '';
                document.getElementById('input-alias').value = result.alias || '';
                document.getElementById('input-line-id').value = result.line_id || '';
                document.getElementById('input-phone').value = result.phone || '';
                document.getElementById('persona-input').value = result.persona || persona;

                alert("✨ 已自动为您填充 AI 生成的角色属性，请点击右上角「保存」！");

            } catch (error) {
                console.error(error);
                alert("API 请求失败，请检查设置或网络。");
            } finally {
                btn.innerText = "通过 API 生成";
                btn.disabled = false;
            }
        }

        document.addEventListener("DOMContentLoaded", () => {
            const searchInput = document.getElementById('line-search-input');
            if (searchInput) {
                searchInput.addEventListener('keypress', function(e) {
                    if (e.key === 'Enter') {
                        searchLineFriend(this.value.trim());
                    }
                });
            }
            document.getElementById('api-url').value = localStorage.getItem('api_url') || '';
            document.getElementById('api-key').value = localStorage.getItem('api_key') || '';
            document.getElementById('api-model').value = localStorage.getItem('api_model') || 'gpt-4o';
            setSearchType('id');
            renderContactsList();
            renderLineFriendsAndChats();
        });

        function openApp(appName) {
            closeAllLineModals();
            closeChatDetail();
            document.querySelectorAll('.app-view').forEach(app => {
                app.classList.remove('active-app');
                app.classList.add('hidden-app');
            });
            const targetApp = document.getElementById(`app-${appName}`);
            if (targetApp) {
                targetApp.classList.remove('hidden-app');
                targetApp.classList.add('active-app');
            }
        }

        function goHome() {
            closeAllLineModals();
            closeCreateCharacterModal();
            closeChatDetail();
            document.querySelectorAll('.app-view').forEach(app => {
                app.classList.remove('active-app');
                app.classList.add('hidden-app');
            });
        }

        function openLineAddModal() {
            const modal = document.getElementById('modal-line-add-friends');
            const sheet = document.getElementById('modal-sheet-content');
            modal.classList.remove('pointer-events-none', 'opacity-0');
            modal.classList.add('opacity-100');
            sheet.classList.remove('slide-down');
            sheet.classList.add('slide-up');
        }

        function openLineSearchModal() {
            const modal = document.getElementById('modal-line-search-friends');
            const sheet = document.getElementById('modal-search-sheet-content');
            modal.classList.remove('pointer-events-none', 'opacity-0');
            modal.classList.add('opacity-100');
            sheet.classList.remove('slide-down');
            sheet.classList.add('slide-up');
        }

        function backToAddFriendsModal() {
            const searchModal = document.getElementById('modal-line-search-friends');
            const searchSheet = document.getElementById('modal-search-sheet-content');
            searchSheet.classList.remove('slide-up');
            searchSheet.classList.add('slide-down');
            searchModal.classList.remove('opacity-100');
            searchModal.classList.add('opacity-0', 'pointer-events-none');
        }

        function closeAllLineModals() {
            backToAddFriendsModal();
            const addModal = document.getElementById('modal-line-add-friends');
            const addSheet = document.getElementById('modal-sheet-content');
            if (addModal && addSheet) {
                addSheet.classList.remove('slide-up');
                addSheet.classList.add('slide-down');
                addModal.classList.remove('opacity-100');
                addModal.classList.add('opacity-0', 'pointer-events-none');
            }
        }

        function setSearchType(type) {
            currentSearchType = type;
            const idOuter = document.getElementById('radio-id-outer');
            const idInner = document.getElementById('radio-id-inner');
            const phoneOuter = document.getElementById('radio-phone-outer');
            const phoneInner = document.getElementById('radio-phone-inner');
            const searchInput = document.getElementById('line-search-input');

            if (type === 'id') {
                idOuter.className = "w-4 h-4 rounded-full border-2 border-[#06C755] flex items-center justify-center p-0.5";
                idInner.className = "w-full h-full rounded-full bg-[#06C755]";
                phoneOuter.className = "w-4 h-4 rounded-full border border-stone-300 flex items-center justify-center p-0.5";
                phoneInner.className = "w-full h-full rounded-full bg-transparent";
                searchInput.placeholder = "输入好友的 ID";
            } else {
                phoneOuter.className = "w-4 h-4 rounded-full border-2 border-[#06C755] flex items-center justify-center p-0.5";
                phoneInner.className = "w-full h-full rounded-full bg-[#06C755]";
                idOuter.className = "w-4 h-4 rounded-full border border-stone-300 flex items-center justify-center p-0.5";
                idInner.className = "w-full h-full rounded-full bg-transparent";
                searchInput.placeholder = "输入好友的电话号码";
            }
        }

        function saveApiConfig() {
            const url = document.getElementById('api-url').value.trim();
            const key = document.getElementById('api-key').value.trim();
            const model = document.getElementById('api-model').value.trim();
            localStorage.setItem('api_url', url);
            localStorage.setItem('api_key', key);
            localStorage.setItem('api_model', model);
            alert("设置已成功保存！");
        }
    </script>
</body>
</html>
