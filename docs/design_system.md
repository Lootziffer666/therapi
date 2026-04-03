<!-- Design System -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>therAPI | Control Panel</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "surface-container": "#edeeee",
                        "error": "#ba1a1a",
                        "primary-container": "#005b63",
                        "on-surface": "#191c1c",
                        "tertiary": "#004247",
                        "on-tertiary-container": "#84d2db",
                        "inverse-surface": "#2e3131",
                        "surface-tint": "#1a6870",
                        "surface-bright": "#f8f9f9",
                        "inverse-on-surface": "#f0f1f1",
                        "on-primary": "#ffffff",
                        "primary": "#004248",
                        "secondary": "#505f78",
                        "on-primary-fixed-variant": "#004f56",
                        "on-surface-variant": "#3f484a",
                        "on-tertiary-fixed": "#002023",
                        "secondary-fixed-dim": "#b8c7e4",
                        "on-secondary-container": "#54637d",
                        "on-tertiary": "#ffffff",
                        "background": "#f8f9f9",
                        "on-tertiary-fixed-variant": "#004f55",
                        "on-secondary-fixed": "#0c1c32",
                        "error-container": "#ffdad6",
                        "surface-container-highest": "#e1e3e3",
                        "on-primary-container": "#8cd0d9",
                        "surface-container-high": "#e7e8e8",
                        "surface-dim": "#d9dada",
                        "primary-fixed-dim": "#8dd2db",
                        "on-secondary": "#ffffff",
                        "inverse-primary": "#8dd2db",
                        "surface-container-lowest": "#ffffff",
                        "outline": "#6f797a",
                        "tertiary-container": "#005b62",
                        "on-error-container": "#93000a",
                        "on-background": "#191c1c",
                        "secondary-container": "#d1e0fe",
                        "surface-container-low": "#f3f4f4",
                        "on-primary-fixed": "#001f23",
                        "tertiary-fixed": "#a1eff9",
                        "on-error": "#ffffff",
                        "surface": "#f8f9f9",
                        "surface-variant": "#e1e3e3",
                        "primary-fixed": "#a9eef7",
                        "secondary-fixed": "#d5e3ff",
                        "tertiary-fixed-dim": "#85d3dc",
                        "on-secondary-fixed-variant": "#394760",
                        "outline-variant": "#bec8ca"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.125rem",
                        "lg": "0.25rem",
                        "xl": "0.5rem",
                        "full": "0.75rem"
                    },
                    "fontFamily": {
                        "headline": ["Inter"],
                        "body": ["Inter"],
                        "label": ["Inter"]
                    }
                },
            },
        }
    </script>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 300, 'GRAD' 0, 'opsz' 24;
        }
        .signature-gradient {
            background: linear-gradient(135deg, #005B63 0%, #7FCDD6 100%);
        }
        .ambient-shadow {
            box-shadow: 0 12px 32px -4px rgba(32, 36, 38, 0.08);
        }
        .backdrop-blur-panel {
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
    </style>
</head>
<body class="bg-surface-container-low font-body text-on-surface">
<!-- SideNavBar Shell -->
<aside class="h-screen w-64 fixed left-0 top-0 bg-[#FAFAFA] dark:bg-slate-900 flex flex-col py-6 z-50">
<div class="px-8 mb-10 flex items-center gap-3">
<div class="w-8 h-8 rounded-lg signature-gradient flex items-center justify-center text-white">
<span class="material-symbols-outlined text-lg" style="font-variation-settings: 'FILL' 1;">api</span>
</div>
<div>
<h1 class="text-xl font-bold text-[#005B63] dark:text-[#7FCDD6] tracking-tighter">therAPI</h1>
<p class="text-[10px] uppercase tracking-widest text-slate-400 font-semibold">API Orchestration</p>
</div>
</div>
<nav class="flex-1 px-4 space-y-2">
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-[#005B63] dark:text-[#7FCDD6] font-bold border-r-4 border-[#005B63] bg-[#005B63]/5 duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">dashboard</span>
<span class="font-inter text-sm font-medium tracking-tight">Control Panel</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 dark:text-slate-400 hover:text-[#005B63] hover:bg-slate-100 transition-colors duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">explore</span>
<span class="font-inter text-sm font-medium tracking-tight">Explorer</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 dark:text-slate-400 hover:text-[#005B63] hover:bg-slate-100 transition-colors duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">compare_arrows</span>
<span class="font-inter text-sm font-medium tracking-tight">Drift</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 dark:text-slate-400 hover:text-[#005B63] hover:bg-slate-100 transition-colors duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">search_check</span>
<span class="font-inter text-sm font-medium tracking-tight">Inspector</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 dark:text-slate-400 hover:text-[#005B63] hover:bg-slate-100 transition-colors duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">download</span>
<span class="font-inter text-sm font-medium tracking-tight">Export</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 dark:text-slate-400 hover:text-[#005B63] hover:bg-slate-100 transition-colors duration-200 ease-in-out" href="#">
<span class="material-symbols-outlined">settings</span>
<span class="font-inter text-sm font-medium tracking-tight">Settings</span>
</a>
</nav>
<div class="mt-auto px-8 py-4">
<div class="flex items-center gap-3">
<img alt="therAPI Logo" class="w-8 h-8 rounded-full bg-slate-200" src="https://lh3.googleusercontent.com/aida-public/AB6AXuBXpYxUtJ6ICm9nXayN20Da0Lm-fsfk-sKUHJDw1qUTzENOf_5MdCe7cwThQJhw6pJCFQ5SyytYycekf8YzEe0mdHDCgbrmqaYXS_tWaIPWmBq1A6etUIo8uN4FAu9MjaJyxa6aIqXbYArdKKPMlyRkx9YNmiotypo0N4yQtId1dXVU8u_cLNizniMZf0N1UF44pglalAHEWZPOUsYMfHDaZ-fE71ukcIajJUYRP3tsgv1cCxgoIsRw7voL66gt_q1aZNti566Wnk0"/>
<div class="flex flex-col">
<span class="text-xs font-bold text-on-surface">v2.4.1-stable</span>
<span class="text-[10px] text-slate-400">Node Cluster: US-East</span>
</div>
</div>
</div>
</aside>
<!-- TopNavBar Shell -->
<header class="fixed top-0 right-0 left-64 h-16 z-40 bg-white/85 backdrop-blur-md flex items-center justify-between px-8 w-full shadow-sm">
<div class="flex items-center gap-4 bg-surface-container-low px-4 py-1.5 rounded-full w-96">
<span class="material-symbols-outlined text-slate-400 text-sm">search</span>
<input class="bg-transparent border-none focus:ring-0 text-sm w-full font-label placeholder:text-slate-400" placeholder="Search endpoints, traces, or schemas..." type="text"/>
</div>
<div class="flex items-center gap-6">
<div class="flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span>
<span class="font-inter text-xs font-semibold text-[#005B63]">Connected</span>
</div>
<div class="h-4 w-[1px] bg-slate-200"></div>
<div class="flex items-center gap-2 text-slate-500">
<span class="material-symbols-outlined text-sm">layers</span>
<span class="font-inter text-xs font-semibold">Production</span>
</div>
<span class="material-symbols-outlined text-slate-600 cursor-pointer hover:opacity-80 transition-opacity">account_circle</span>
</div>
</header>
<!-- Main Content Stage -->
<main class="ml-64 pt-24 px-12 pb-12">
<!-- Header & Quick Actions -->
<div class="flex items-end justify-between mb-8">
<div>
<h2 class="text-3xl font-extrabold text-[#005B63] tracking-tighter mb-1">Control Panel</h2>
<p class="text-sm text-slate-500 font-medium">Monitoring active proxy capture and schema discovery.</p>
</div>
<div class="flex items-center gap-3">
<button class="px-5 py-2.5 bg-surface-container-lowest text-[#005B63] text-sm font-bold rounded-xl ambient-shadow hover:bg-slate-50 transition-colors flex items-center gap-2 border border-[#E7E8E8]/40">
<span class="material-symbols-outlined text-lg">description</span>
                    Export OpenAPI
                </button>
<button class="px-5 py-2.5 bg-surface-container-lowest text-[#005B63] text-sm font-bold rounded-xl ambient-shadow hover:bg-slate-50 transition-colors flex items-center gap-2 border border-[#E7E8E8]/40">
<span class="material-symbols-outlined text-lg">auto_awesome</span>
                    Generate Summary
                </button>
<button class="px-6 py-2.5 text-sm font-bold rounded-xl ambient-shadow flex items-center gap-2" style="background-color: #C92A2A; color: #F4F7F8;">
<span class="material-symbols-outlined text-lg" style="font-variation-settings: 'FILL' 1;">stop_circle</span>
                    Stop Capture
                </button>
</div>
</div>
<!-- Bento Grid Layout -->
<div class="grid grid-cols-12 gap-8 mb-8">
<!-- Proxy Status Card -->
<div class="col-span-4 bg-[#FAFAFA] rounded-xl p-6 ambient-shadow relative overflow-hidden flex flex-col justify-between min-h-[220px]">
<div class="relative z-10">
<div class="flex items-center justify-between mb-4">
<span class="text-[10px] font-bold tracking-widest text-slate-400 uppercase">System Status</span>
<div class="px-3 py-1 bg-emerald-100 text-emerald-700 text-[10px] font-extrabold rounded-full flex items-center gap-1.5">
<span class="w-1.5 h-1.5 rounded-full bg-emerald-500"></span>
                            ONLINE
                        </div>
</div>
<div class="mb-4">
<h3 class="text-slate-400 text-xs font-semibold mb-1">Proxy Host</h3>
<p class="text-xl font-bold text-on-surface">proxy.internal.therapi.io</p>
</div>
</div>
<div class="grid grid-cols-2 gap-4 relative z-10 pt-4 border-t border-slate-100">
<div>
<p class="text-[10px] font-bold text-slate-400 uppercase tracking-wider mb-0.5">Port</p>
<p class="text-lg font-bold text-[#005B63]">8443</p>
</div>
<div>
<p class="text-[10px] font-bold text-slate-400 uppercase tracking-wider mb-0.5">Uptime</p>
<p class="text-lg font-bold text-on-surface">14h 22m</p>
</div>
</div>
<!-- Abstract visual element -->
<div class="absolute -bottom-6 -right-6 w-32 h-32 opacity-10">
<span class="material-symbols-outlined text-8xl" style="font-variation-settings: 'wght' 700;">router</span>
</div>
</div>
<!-- Capture Configuration -->
<div class="col-span-5 bg-[#FAFAFA] rounded-xl p-6 ambient-shadow flex flex-col min-h-[220px]">
<div class="flex items-center gap-2 mb-6">
<span class="material-symbols-outlined text-[#005B63]">settings_input_component</span>
<h3 class="text-sm font-bold text-on-surface">Capture Configuration</h3>
</div>
<div class="space-y-4">
<div class="bg-surface-container-low p-4 rounded-lg">
<div class="flex items-center justify-between mb-2">
<span class="text-[10px] font-bold text-slate-500 uppercase tracking-tighter">Base Target URL</span>
<span class="material-symbols-outlined text-xs text-[#005B63] cursor-pointer">edit</span>
</div>
<p class="text-sm font-mono text-on-surface truncate">https://api.production-v1.prod/v2</p>
</div>
<div class="bg-surface-container-low p-4 rounded-lg">
<div class="flex items-center justify-between mb-2">
<span class="text-[10px] font-bold text-slate-500 uppercase tracking-tighter">Store Path</span>
<span class="material-symbols-outlined text-xs text-[#005B63] cursor-pointer">folder</span>
</div>
<p class="text-sm font-mono text-on-surface truncate">/mnt/storage/captures/daily_run_01</p>
</div>
</div>
</div>
<!-- Node Stability Graph (Synthetic Canvas) -->
<div class="col-span-3 bg-[#1F2E45] rounded-xl p-6 ambient-shadow flex flex-col justify-between overflow-hidden relative">
<div class="relative z-10">
<h3 class="text-white/80 text-xs font-bold uppercase tracking-widest mb-1">Node Stability</h3>
<p class="text-2xl font-extrabold text-white">99.98%</p>
</div>
<!-- Simulated Graph -->
<div class="mt-4 flex items-end gap-1 h-24 relative z-10">
<div class="flex-1 bg-[#7FCDD6]/30 h-[60%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/40 h-[75%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/30 h-[65%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/50 h-[80%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/40 h-[70%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/60 h-[90%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/50 h-[85%] rounded-t-sm"></div>
<div class="flex-1 bg-[#7FCDD6]/80 h-[95%] rounded-t-sm animate-pulse"></div>
</div>
<div class="flex justify-between items-center text-[10px] font-bold text-white/40 mt-3 uppercase tracking-tighter">
<span>Latency: 14ms</span>
<span>Load: 4.2%</span>
</div>
<!-- Background decor -->
<div class="absolute inset-0 bg-gradient-to-br from-transparent to-white/5 pointer-events-none"></div>
</div>
</div>
<!-- Endpoint Overview Table -->
<section class="bg-[#FAFAFA] rounded-2xl ambient-shadow overflow-hidden">
<div class="px-8 py-6 flex items-center justify-between border-b border-slate-100">
<div>
<h3 class="text-lg font-bold text-on-surface">Endpoint Overview</h3>
<p class="text-xs text-slate-400 font-medium">Discovered schemas from current traffic stream</p>
</div>
<div class="flex items-center gap-2">
<div class="flex -space-x-2">
<div class="w-6 h-6 rounded-full bg-slate-200 border-2 border-white flex items-center justify-center text-[8px] font-bold">JD</div>
<div class="w-6 h-6 rounded-full bg-slate-300 border-2 border-white flex items-center justify-center text-[8px] font-bold">AK</div>
<div class="w-6 h-6 rounded-full bg-slate-100 border-2 border-white flex items-center justify-center text-[8px] font-bold">+4</div>
</div>
<button class="ml-4 p-2 text-slate-400 hover:text-[#005B63] transition-colors">
<span class="material-symbols-outlined">filter_list</span>
</button>
</div>
</div>
<table class="w-full text-left border-collapse">
<thead>
<tr class="text-[10px] uppercase tracking-widest text-slate-400 font-bold bg-surface-container-low/50">
<th class="px-8 py-4">Method</th>
<th class="px-4 py-4">Path</th>
<th class="px-4 py-4">Samples</th>
<th class="px-4 py-4">Versions</th>
<th class="px-4 py-4">Last Changed</th>
<th class="px-8 py-4 text-right">Action</th>
</tr>
</thead>
<tbody class="divide-y divide-slate-50">
<!-- Row 1 -->
<tr class="group hover:bg-slate-50 transition-colors">
<td class="px-8 py-5">
<span class="px-2.5 py-1 bg-emerald-100 text-emerald-700 text-[10px] font-bold rounded-md">GET</span>
</td>
<td class="px-4 py-5">
<span class="text-sm font-mono text-on-surface">/users/{user_id}/profile</span>
</td>
<td class="px-4 py-5 text-sm text-slate-600 font-medium">1,422</td>
<td class="px-4 py-5">
<div class="flex items-center gap-1.5">
<span class="w-2 h-2 rounded-full bg-slate-300"></span>
<span class="text-xs font-bold text-slate-500">v1.2</span>
</div>
</td>
<td class="px-4 py-5 text-xs text-slate-400">2 minutes ago</td>
<td class="px-8 py-5 text-right">
<span class="material-symbols-outlined text-slate-300 group-hover:text-[#005B63] cursor-pointer">arrow_forward_ios</span>
</td>
</tr>
<!-- Row 2 -->
<tr class="group hover:bg-slate-50 transition-colors">
<td class="px-8 py-5">
<span class="px-2.5 py-1 bg-blue-100 text-blue-700 text-[10px] font-bold rounded-md">POST</span>
</td>
<td class="px-4 py-5">
<span class="text-sm font-mono text-on-surface">/auth/token/refresh</span>
</td>
<td class="px-4 py-5 text-sm text-slate-600 font-medium">843</td>
<td class="px-4 py-5">
<div class="flex items-center gap-1.5">
<span class="w-2 h-2 rounded-full bg-[#005B63]"></span>
<span class="text-xs font-bold text-on-surface">v2.0</span>
</div>
</td>
<td class="px-4 py-5 text-xs text-slate-400">14 minutes ago</td>
<td class="px-8 py-5 text-right">
<span class="material-symbols-outlined text-slate-300 group-hover:text-[#005B63] cursor-pointer">arrow_forward_ios</span>
</td>
</tr>
<!-- Row 3 -->
<tr class="group hover:bg-slate-50 transition-colors">
<td class="px-8 py-5">
<span class="px-2.5 py-1 bg-amber-100 text-amber-700 text-[10px] font-bold rounded-md">PATCH</span>
</td>
<td class="px-4 py-5">
<span class="text-sm font-mono text-on-surface">/organization/{id}/billing</span>
</td>
<td class="px-4 py-5 text-sm text-slate-600 font-medium">12</td>
<td class="px-4 py-5">
<div class="flex items-center gap-1.5">
<span class="w-2 h-2 rounded-full bg-slate-300"></span>
<span class="text-xs font-bold text-slate-500">v0.9-alpha</span>
</div>
</td>
<td class="px-4 py-5 text-xs text-slate-400">1 hour ago</td>
<td class="px-8 py-5 text-right">
<span class="material-symbols-outlined text-slate-300 group-hover:text-[#005B63] cursor-pointer">arrow_forward_ios</span>
</td>
</tr>
<!-- Row 4 -->
<tr class="group hover:bg-slate-50 transition-colors">
<td class="px-8 py-5">
<span class="px-2.5 py-1 bg-emerald-100 text-emerald-700 text-[10px] font-bold rounded-md">GET</span>
</td>
<td class="px-4 py-5">
<span class="text-sm font-mono text-on-surface">/search/global?q={query}</span>
</td>
<td class="px-4 py-5 text-sm text-slate-600 font-medium">5,910</td>
<td class="px-4 py-5">
<div class="flex items-center gap-1.5">
<span class="w-2 h-2 rounded-full bg-[#005B63]"></span>
<span class="text-xs font-bold text-on-surface">v1.2</span>
</div>
</td>
<td class="px-4 py-5 text-xs text-slate-400">4 minutes ago</td>
<td class="px-8 py-5 text-right">
<span class="material-symbols-outlined text-slate-300 group-hover:text-[#005B63] cursor-pointer">arrow_forward_ios</span>
</td>
</tr>
</tbody>
</table>
<div class="p-6 bg-surface-container-low/30 text-center">
<button class="text-xs font-bold text-[#005B63] uppercase tracking-widest hover:underline">View All 128 Endpoints</button>
</div>
</section>
</main>
<!-- Floating System Analytics Popover (Asymmetric Element) -->
<div class="fixed bottom-12 right-12 w-80 bg-white/90 backdrop-blur-panel rounded-2xl ambient-shadow p-6 border border-white/50 z-50">
<div class="flex items-center justify-between mb-4">
<h4 class="text-sm font-extrabold text-[#005B63]">Real-time Analytics</h4>
<span class="material-symbols-outlined text-slate-300 text-sm">open_in_full</span>
</div>
<div class="space-y-4">
<div>
<div class="flex justify-between text-[10px] font-bold text-slate-500 mb-1">
<span>MEMORY USAGE</span>
<span>1.2 GB / 4.0 GB</span>
</div>
<div class="w-full h-1.5 bg-slate-100 rounded-full overflow-hidden">
<div class="h-full bg-[#005B63] rounded-full" style="width: 30%"></div>
</div>
</div>
<div class="flex gap-4">
<div class="flex-1 bg-surface-container-low rounded-lg p-3 text-center">
<p class="text-[8px] font-extrabold text-slate-400 uppercase tracking-tighter">Req / Sec</p>
<p class="text-lg font-bold text-[#005B63]">42.8</p>
</div>
<div class="flex-1 bg-surface-container-low rounded-lg p-3 text-center">
<p class="text-[8px] font-extrabold text-slate-400 uppercase tracking-tighter">Errors</p>
<p class="text-lg font-bold text-error">0.02%</p>
</div>
</div>
</div>
</div>
</body></html>

<!-- Control Panel (Updated Button) -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>therAPI | Capture Inspector</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            "colors": {
                    "surface-container": "#edeeee",
                    "error": "#ba1a1a",
                    "primary-container": "#005b63",
                    "on-surface": "#191c1c",
                    "tertiary": "#004247",
                    "on-tertiary-container": "#84d2db",
                    "inverse-surface": "#2e3131",
                    "surface-tint": "#1a6870",
                    "surface-bright": "#f8f9f9",
                    "inverse-on-surface": "#f0f1f1",
                    "on-primary": "#ffffff",
                    "primary": "#004248",
                    "secondary": "#505f78",
                    "on-primary-fixed-variant": "#004f56",
                    "on-surface-variant": "#3f484a",
                    "on-tertiary-fixed": "#002023",
                    "secondary-fixed-dim": "#b8c7e4",
                    "on-secondary-container": "#54637d",
                    "on-tertiary": "#ffffff",
                    "background": "#f8f9f9",
                    "on-tertiary-fixed-variant": "#004f55",
                    "on-secondary-fixed": "#0c1c32",
                    "error-container": "#ffdad6",
                    "surface-container-highest": "#e1e3e3",
                    "on-primary-container": "#8cd0d9",
                    "surface-container-high": "#e7e8e8",
                    "surface-dim": "#d9dada",
                    "primary-fixed-dim": "#8dd2db",
                    "on-secondary": "#ffffff",
                    "inverse-primary": "#8dd2db",
                    "surface-container-lowest": "#ffffff",
                    "outline": "#6f797a",
                    "tertiary-container": "#005b62",
                    "on-error-container": "#93000a",
                    "on-background": "#191c1c",
                    "secondary-container": "#d1e0fe",
                    "surface-container-low": "#f3f4f4",
                    "on-primary-fixed": "#001f23",
                    "tertiary-fixed": "#a1eff9",
                    "on-error": "#ffffff",
                    "surface": "#f8f9f9",
                    "surface-variant": "#e1e3e3",
                    "primary-fixed": "#a9eef7",
                    "secondary-fixed": "#d5e3ff",
                    "tertiary-fixed-dim": "#85d3dc",
                    "on-secondary-fixed-variant": "#394760",
                    "outline-variant": "#bec8ca"
            },
            "borderRadius": {
                    "DEFAULT": "0.125rem",
                    "lg": "0.25rem",
                    "xl": "0.5rem",
                    "full": "0.75rem"
            },
            "fontFamily": {
                    "headline": ["Inter"],
                    "body": ["Inter"],
                    "label": ["Inter"]
            }
          },
        },
      }
    </script>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 20;
            font-size: 20px;
        }
        .signature-gradient {
            background: linear-gradient(135deg, #005B63 0%, #7FCDD6 100%);
        }
        .code-panel {
            background-color: #1B2740;
            color: #DDE6EE;
        }
        .syntax-key { color: #84d2db; }
        .syntax-string { color: #91A2B2; }
    </style>
</head>
<body class="bg-surface-container-low font-body text-on-surface">
<!-- SideNavBar (Shared Component) -->
<aside class="h-screen w-64 fixed left-0 top-0 bg-[#FAFAFA] dark:bg-slate-900 flex flex-col py-6">
<div class="px-6 mb-10 flex items-center gap-3">
<div class="w-8 h-8 rounded-lg signature-gradient flex items-center justify-center text-white">
<span class="material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">api</span>
</div>
<div>
<h1 class="text-xl font-bold text-[#005B63] dark:text-[#7FCDD6] tracking-tighter">therAPI</h1>
<p class="text-[10px] uppercase tracking-widest text-slate-400 font-semibold">API Orchestration</p>
</div>
</div>
<nav class="flex-1 space-y-1 px-3">
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-slate-500 hover:bg-slate-100 transition-colors font-medium text-sm" href="#">
<span class="material-symbols-outlined">dashboard</span>
                Control Panel
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-slate-500 hover:bg-slate-100 transition-colors font-medium text-sm" href="#">
<span class="material-symbols-outlined">explore</span>
                Explorer
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-slate-500 hover:bg-slate-100 transition-colors font-medium text-sm" href="#">
<span class="material-symbols-outlined">compare_arrows</span>
                Drift
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-[#005B63] dark:text-[#7FCDD6] font-bold border-r-4 border-[#005B63] bg-[#005B63]/5 font-medium text-sm" href="#">
<span class="material-symbols-outlined">search_check</span>
                Inspector
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-slate-500 hover:bg-slate-100 transition-colors font-medium text-sm" href="#">
<span class="material-symbols-outlined">download</span>
                Export
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-xl text-slate-500 hover:bg-slate-100 transition-colors font-medium text-sm" href="#">
<span class="material-symbols-outlined">settings</span>
                Settings
            </a>
</nav>
<div class="px-6 mt-auto">
<div class="p-4 bg-white rounded-2xl shadow-sm border border-slate-100">
<p class="text-xs text-slate-400 mb-2">Usage Limit</p>
<div class="h-1.5 w-full bg-slate-100 rounded-full overflow-hidden">
<div class="h-full bg-[#005B63] w-3/4"></div>
</div>
<p class="text-[10px] mt-2 font-bold text-[#005B63]">75% of 1M requests</p>
</div>
</div>
</aside>
<!-- TopNavBar (Shared Component) -->
<header class="fixed top-0 right-0 left-64 h-16 z-40 bg-white/85 backdrop-blur-md flex items-center justify-between px-8">
<div class="flex items-center gap-4 flex-1">
<div class="relative w-96">
<span class="material-symbols-outlined absolute left-3 top-1/2 -translate-y-1/2 text-slate-400">search</span>
<input class="w-full bg-surface-container-low border-none rounded-full py-2 pl-10 pr-4 text-sm focus:ring-2 focus:ring-[#005B63]/20" placeholder="Search captures or trace IDs..." type="text"/>
</div>
</div>
<div class="flex items-center gap-6">
<div class="flex items-center gap-2 px-3 py-1 bg-green-50 rounded-full">
<span class="w-2 h-2 rounded-full bg-green-500"></span>
<span class="text-xs font-semibold text-green-700">Connected</span>
</div>
<div class="h-8 w-px bg-slate-200"></div>
<div class="flex items-center gap-3 cursor-pointer">
<span class="text-sm font-semibold text-slate-700">Production</span>
<span class="material-symbols-outlined text-slate-400">account_circle</span>
</div>
</div>
</header>
<!-- Main Content Canvas -->
<main class="ml-64 pt-24 px-8 pb-12">
<!-- Request Header -->
<section class="mb-8">
<div class="flex items-end justify-between mb-4">
<div>
<nav class="flex items-center gap-2 text-xs text-slate-400 font-medium mb-2">
<span>Captures</span>
<span class="material-symbols-outlined text-[12px]">chevron_right</span>
<span class="text-[#005B63]">Inspector</span>
</nav>
<h2 class="text-3xl font-extrabold tracking-tight text-[#1F2E45]">Capture Inspector</h2>
</div>
<button class="signature-gradient text-white px-5 py-2.5 rounded-xl font-bold text-sm shadow-lg shadow-[#005B63]/20 flex items-center gap-2">
<span class="material-symbols-outlined">refresh</span>
                    Replay Request
                </button>
</div>
<div class="bg-surface-container-lowest rounded-2xl p-6 shadow-sm flex items-center justify-between">
<div class="flex items-center gap-6">
<div class="bg-[#1F2E45] text-[#7FCDD6] px-4 py-1.5 rounded-lg font-bold tracking-wider text-sm">POST</div>
<div class="font-mono text-sm text-slate-600 bg-slate-50 px-3 py-1.5 rounded-md border border-slate-100">
                        https://api.therapi.io/v1/orchestrate/deployments/nodes/query
                    </div>
</div>
<div class="flex items-center gap-4">
<div class="text-right">
<div class="text-[10px] uppercase font-bold text-slate-400">Status</div>
<div class="text-lg font-bold text-green-600">200 OK</div>
</div>
<div class="w-px h-10 bg-slate-100"></div>
<div class="text-right">
<div class="text-[10px] uppercase font-bold text-slate-400">Latency</div>
<div class="text-lg font-bold text-slate-800">104ms</div>
</div>
</div>
</div>
</section>
<!-- PII Shield Notice -->
<section class="mb-8">
<div class="bg-[#004247] text-white p-4 rounded-2xl flex items-center justify-between">
<div class="flex items-center gap-3">
<div class="w-10 h-10 rounded-full bg-white/10 flex items-center justify-center">
<span class="material-symbols-outlined text-[#7FCDD6]" style="font-variation-settings: 'FILL' 1;">shield_with_heart</span>
</div>
<div>
<p class="font-bold text-sm">PII Shield Active</p>
<p class="text-xs text-[#84d2db]">3 sensitive fields redacted from this capture</p>
</div>
</div>
<button class="text-xs font-bold px-4 py-2 bg-white/10 hover:bg-white/20 rounded-lg transition-colors">Manage Masking</button>
</div>
</section>
<!-- Bento Grid: Insights & Security -->
<div class="grid grid-cols-3 gap-6 mb-8">
<!-- Network Insights Card -->
<div class="col-span-2 bg-surface-container-lowest rounded-2xl p-8 shadow-sm">
<div class="flex items-center justify-between mb-8">
<h3 class="text-lg font-bold text-[#1F2E45]">Network Insights</h3>
<span class="material-symbols-outlined text-slate-300">speed</span>
</div>
<div class="space-y-6">
<div class="relative">
<div class="flex justify-between text-xs font-bold text-slate-400 mb-2 uppercase tracking-wide">
<span>DNS Lookup</span>
<span class="text-[#005B63]">12ms</span>
</div>
<div class="h-2 w-full bg-slate-50 rounded-full overflow-hidden">
<div class="h-full signature-gradient" style="width: 12%"></div>
</div>
</div>
<div class="relative">
<div class="flex justify-between text-xs font-bold text-slate-400 mb-2 uppercase tracking-wide">
<span>TCP Handshake</span>
<span class="text-[#005B63]">28ms</span>
</div>
<div class="h-2 w-full bg-slate-50 rounded-full overflow-hidden">
<div class="h-full signature-gradient" style="width: 28%"></div>
</div>
</div>
<div class="relative">
<div class="flex justify-between text-xs font-bold text-slate-400 mb-2 uppercase tracking-wide">
<span>TLS Negotiation</span>
<span class="text-[#005B63]">64ms</span>
</div>
<div class="h-2 w-full bg-slate-50 rounded-full overflow-hidden">
<div class="h-full signature-gradient" style="width: 64%"></div>
</div>
</div>
</div>
</div>
<!-- Security Profile -->
<div class="col-span-1 bg-surface-container-lowest rounded-2xl p-8 shadow-sm relative overflow-hidden">
<div class="absolute -right-4 -top-4 w-24 h-24 bg-[#005B63]/5 rounded-full blur-2xl"></div>
<h3 class="text-lg font-bold text-[#1F2E45] mb-6">Security Profile</h3>
<div class="space-y-4">
<div class="flex items-center justify-between p-3 bg-slate-50 rounded-xl">
<span class="text-sm font-medium text-slate-500">Encryption</span>
<span class="text-xs font-bold text-[#005B63] bg-[#005B63]/10 px-2 py-1 rounded">TLS 1.3</span>
</div>
<div class="flex items-center justify-between p-3 bg-slate-50 rounded-xl">
<span class="text-sm font-medium text-slate-500">HSTS</span>
<span class="material-symbols-outlined text-green-500 text-sm">check_circle</span>
</div>
<div class="flex items-center justify-between p-3 bg-slate-50 rounded-xl">
<span class="text-sm font-medium text-slate-500">XSS Protection</span>
<span class="material-symbols-outlined text-green-500 text-sm">check_circle</span>
</div>
<div class="flex items-center justify-between p-3 bg-slate-50 rounded-xl">
<span class="text-sm font-medium text-slate-500">CORS</span>
<span class="text-xs font-bold text-amber-600 bg-amber-50 px-2 py-1 rounded">Restricted</span>
</div>
</div>
</div>
</div>
<!-- JSON Code Panels -->
<div class="grid grid-cols-2 gap-6">
<!-- Request Body -->
<div class="rounded-2xl overflow-hidden shadow-xl">
<div class="bg-[#1F2E45] px-6 py-4 flex items-center justify-between border-b border-white/5">
<div class="flex items-center gap-3">
<span class="material-symbols-outlined text-[#7FCDD6]">upload</span>
<h4 class="text-sm font-bold text-white tracking-wide">Request Body</h4>
</div>
<button class="text-white/40 hover:text-white transition-colors">
<span class="material-symbols-outlined text-sm">content_copy</span>
</button>
</div>
<div class="code-panel p-6 font-mono text-sm h-[400px] overflow-auto leading-relaxed">
<pre><code>{
  <span class="syntax-key">"node_id"</span>: <span class="syntax-string">"nd-8829-axp"</span>,
  <span class="syntax-key">"operation"</span>: <span class="syntax-string">"sync_state"</span>,
  <span class="syntax-key">"context"</span>: {
    <span class="syntax-key">"region"</span>: <span class="syntax-string">"us-east-1"</span>,
    <span class="syntax-key">"tier"</span>: <span class="syntax-string">"enterprise"</span>,
    <span class="syntax-key">"auth_token"</span>: <span class="syntax-string">"********************"</span>
  },
  <span class="syntax-key">"parameters"</span>: {
    <span class="syntax-key">"depth"</span>: <span class="syntax-string">12</span>,
    <span class="syntax-key">"verbose"</span>: <span class="syntax-string">true</span>
  }
}</code></pre>
</div>
</div>
<!-- Response Body -->
<div class="rounded-2xl overflow-hidden shadow-xl">
<div class="bg-[#1F2E45] px-6 py-4 flex items-center justify-between border-b border-white/5">
<div class="flex items-center gap-3">
<span class="material-symbols-outlined text-[#7FCDD6]">download</span>
<h4 class="text-sm font-bold text-white tracking-wide">Response Body</h4>
</div>
<button class="text-white/40 hover:text-white transition-colors">
<span class="material-symbols-outlined text-sm">content_copy</span>
</button>
</div>
<div class="code-panel p-6 font-mono text-sm h-[400px] overflow-auto leading-relaxed">
<pre><code>{
  <span class="syntax-key">"status"</span>: <span class="syntax-string">"success"</span>,
  <span class="syntax-key">"timestamp"</span>: <span class="syntax-string">"2023-11-24T14:22:01.004Z"</span>,
  <span class="syntax-key">"data"</span>: {
    <span class="syntax-key">"sync_id"</span>: <span class="syntax-string">"sync_099127635"</span>,
    <span class="syntax-key">"nodes_affected"</span>: <span class="syntax-string">42</span>,
    <span class="syntax-key">"drift_detected"</span>: <span class="syntax-string">false</span>,
    <span class="syntax-key">"payload_hash"</span>: <span class="syntax-string">"sha256:0x882a...e12"</span>
  },
  <span class="syntax-key">"meta"</span>: {
    <span class="syntax-key">"processing_time"</span>: <span class="syntax-string">"88ms"</span>,
    <span class="syntax-key">"server_id"</span>: <span class="syntax-string">"therapi-edge-04"</span>
  }
}</code></pre>
</div>
</div>
</div>
</main>
<!-- Background Decorative Element -->
<div class="fixed top-0 right-0 -z-10 opacity-20 pointer-events-none">
<svg fill="none" height="600" viewbox="0 0 600 600" width="600" xmlns="http://www.w3.org/2000/svg">
<circle cx="300" cy="300" fill="url(#paint0_radial_1_1)" r="300"></circle>
<defs>
<radialgradient cx="0" cy="0" gradienttransform="translate(300 300) rotate(90) scale(300)" gradientunits="userSpaceOnUse" id="paint0_radial_1_1" r="1">
<stop stop-color="#7FCDD6"></stop>
<stop offset="1" stop-color="white" stop-opacity="0"></stop>
</radialgradient>
</defs>
</svg>
</div>
</body></html>

<!-- image.png -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Schema Drift Analysis | therAPI</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&amp;family=Manrope:wght@600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "surface-container-highest": "#e1e3e3",
                        "tertiary-fixed": "#d6e5e5",
                        "tertiary-container": "#576565",
                        "on-secondary-fixed-variant": "#00504b",
                        "surface-dim": "#d8dada",
                        "secondary-fixed-dim": "#90d3cb",
                        "secondary-fixed": "#acefe7",
                        "surface-container-low": "#f2f4f4",
                        "secondary": "#236863",
                        "surface": "#f8fafa",
                        "on-tertiary-fixed-variant": "#3c494a",
                        "surface-bright": "#f8fafa",
                        "on-primary-container": "#9becf7",
                        "primary-container": "#006d77",
                        "inverse-primary": "#82d3de",
                        "background": "#f8fafa",
                        "on-tertiary-container": "#d3e2e2",
                        "on-secondary-container": "#286d67",
                        "on-surface": "#191c1d",
                        "primary-fixed-dim": "#82d3de",
                        "surface-variant": "#e1e3e3",
                        "tertiary-fixed-dim": "#bbc9c9",
                        "surface-container": "#eceeee",
                        "secondary-container": "#a9ece5",
                        "outline": "#6f797a",
                        "on-surface-variant": "#3e494a",
                        "on-tertiary-fixed": "#101e1e",
                        "on-primary": "#ffffff",
                        "surface-container-lowest": "#ffffff",
                        "inverse-on-surface": "#eff1f1",
                        "tertiary": "#3f4d4d",
                        "on-primary-fixed": "#001f23",
                        "on-secondary-fixed": "#00201e",
                        "inverse-surface": "#2e3131",
                        "on-tertiary": "#ffffff",
                        "primary-fixed": "#9ff0fb",
                        "outline-variant": "#bec8ca",
                        "surface-container-high": "#e6e8e9",
                        "surface-tint": "#006972",
                        "on-background": "#191c1d",
                        "on-error": "#ffffff",
                        "on-error-container": "#93000a",
                        "error-container": "#ffdad6",
                        "on-secondary": "#ffffff",
                        "error": "#ba1a1a",
                        "primary": "#00535b",
                        "on-primary-fixed-variant": "#004f56"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "fontFamily": {
                        "headline": ["Manrope"],
                        "body": ["Inter"],
                        "label": ["Inter"]
                    }
                },
            },
        }
    </script>
<style>
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
            vertical-align: middle;
        }
        body { font-family: 'Inter', sans-serif; }
        h1, h2, h3 { font-family: 'Manrope', sans-serif; }
        .glass-panel {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(20px);
        }
        .code-font { font-family: 'ui-monospace', 'SFMono-Regular', 'Menlo', 'Monaco', 'Consolas', monospace; }
    </style>
</head>
<body class="bg-background text-on-surface">
<!-- SideNavBar (Shared Component) -->
<aside class="bg-[#f2f4f4] dark:bg-slate-900 h-screen w-64 fixed left-0 top-0 flex flex-col py-8 px-4 z-50">
<div class="mb-10 px-4">
<h1 class="text-2xl font-bold tracking-tight text-[#00535b] dark:text-[#006d77]">therAPI</h1>
<p class="text-[10px] font-semibold uppercase tracking-wider text-[#3e494a] mt-1">v2.4.0-stable</p>
</div>
<nav class="flex-grow space-y-1">
<a class="flex items-center gap-3 px-4 py-3 text-[#3e494a] dark:text-slate-400 font-medium hover:text-[#00535b] hover:bg-white/50 dark:hover:bg-slate-800 transition-colors rounded-lg group active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="dashboard">dashboard</span>
<span class="text-sm">Control Panel</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 text-[#3e494a] dark:text-slate-400 font-medium hover:text-[#00535b] hover:bg-white/50 dark:hover:bg-slate-800 transition-colors rounded-lg group active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="explore">explore</span>
<span class="text-sm">Explorer</span>
</a>
<!-- Active State: Drift -->
<a class="flex items-center gap-3 px-4 py-3 text-[#00535b] dark:text-[#006d77] font-bold border-r-4 border-[#00535b] bg-white/50 dark:bg-slate-800 rounded-l-lg active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="compare_arrows">compare_arrows</span>
<span class="text-sm">Drift</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 text-[#3e494a] dark:text-slate-400 font-medium hover:text-[#00535b] hover:bg-white/50 dark:hover:bg-slate-800 transition-colors rounded-lg group active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="search_check">search_check</span>
<span class="text-sm">Inspector</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 text-[#3e494a] dark:text-slate-400 font-medium hover:text-[#00535b] hover:bg-white/50 dark:hover:bg-slate-800 transition-colors rounded-lg group active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="download">download</span>
<span class="text-sm">Export</span>
</a>
<a class="flex items-center gap-3 px-4 py-3 text-[#3e494a] dark:text-slate-400 font-medium hover:text-[#00535b] hover:bg-white/50 dark:hover:bg-slate-800 transition-colors rounded-lg group active:scale-95" href="#">
<span class="material-symbols-outlined" data-icon="settings">settings</span>
<span class="text-sm">Settings</span>
</a>
</nav>
<div class="mt-auto px-4">
<button class="w-full py-3 bg-primary text-on-primary rounded-xl font-semibold flex items-center justify-center gap-2 shadow-sm hover:bg-primary-container transition-all active:scale-95">
<span class="material-symbols-outlined text-sm" data-icon="add">add</span>
                New Request
            </button>
</div>
</aside>
<!-- TopNavBar (Shared Component) -->
<header class="fixed top-0 right-0 left-64 h-16 bg-white/85 dark:bg-slate-950/85 backdrop-blur-md flex justify-between items-center px-8 w-full z-40 transition-opacity duration-200">
<div class="flex items-center gap-4 flex-1">
<div class="relative w-full max-w-md">
<span class="material-symbols-outlined absolute left-3 top-1/2 -translate-y-1/2 text-outline" data-icon="search">search</span>
<input class="w-full bg-surface-container-low border-none rounded-lg pl-10 pr-4 py-2 text-sm focus:ring-2 focus:ring-primary" placeholder="Search schema versions..." type="text"/>
</div>
</div>
<div class="flex items-center gap-6">
<div class="flex items-center gap-2">
<span class="h-2 w-2 rounded-full bg-emerald-500 animate-pulse"></span>
<span class="text-xs font-semibold text-primary uppercase tracking-widest">Connected</span>
</div>
<div class="h-4 w-[1px] bg-outline-variant"></div>
<span class="text-xs font-bold text-on-surface-variant">Production</span>
<div class="flex items-center gap-3">
<button class="p-2 hover:bg-[#f2f4f4] dark:hover:bg-slate-800 rounded-lg transition-colors">
<span class="material-symbols-outlined text-on-surface-variant" data-icon="notifications">notifications</span>
</button>
<button class="p-2 hover:bg-[#f2f4f4] dark:hover:bg-slate-800 rounded-lg transition-colors">
<span class="material-symbols-outlined text-on-surface-variant" data-icon="account_circle">account_circle</span>
</button>
</div>
</div>
</header>
<!-- Main Content Canvas -->
<main class="ml-64 pt-24 pb-12 px-8 min-h-screen">
<div class="max-w-7xl mx-auto space-y-8">
<!-- Page Header -->
<div class="flex justify-between items-end">
<div>
<h2 class="text-3xl font-extrabold tracking-tight text-on-surface">Schema Drift Analysis</h2>
<p class="text-on-surface-variant mt-1">Comparing <span class="font-bold text-primary">v1.0.1</span> to <span class="font-bold text-primary">v1.0.4 (Current)</span></p>
</div>
<div class="flex gap-3">
<button class="px-4 py-2 bg-surface-container-lowest text-primary border border-outline-variant/30 rounded-lg text-sm font-semibold hover:bg-surface-container-low transition-colors">
                        Download Report
                    </button>
<button class="px-4 py-2 bg-primary text-on-primary rounded-lg text-sm font-semibold hover:bg-primary-container transition-colors">
                        Approve Schema Change
                    </button>
</div>
</div>
<!-- Bento Grid Layout -->
<div class="grid grid-cols-12 gap-6">
<!-- 1. Comparison Summary Cards -->
<div class="col-span-12 md:col-span-3 h-full">
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm space-y-4 border border-outline-variant/10">
<div class="flex items-center justify-between">
<span class="text-xs font-bold uppercase tracking-widest text-on-surface-variant">Fields Added</span>
<span class="material-symbols-outlined text-emerald-600" data-icon="add_circle">add_circle</span>
</div>
<div class="text-4xl font-bold text-emerald-700">+14</div>
<div class="h-1 w-full bg-surface-container-low rounded-full overflow-hidden">
<div class="h-full bg-emerald-500 w-3/4"></div>
</div>
</div>
</div>
<div class="col-span-12 md:col-span-3">
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm space-y-4 border border-outline-variant/10">
<div class="flex items-center justify-between">
<span class="text-xs font-bold uppercase tracking-widest text-on-surface-variant">Fields Removed</span>
<span class="material-symbols-outlined text-error" data-icon="do_not_disturb_on">do_not_disturb_on</span>
</div>
<div class="text-4xl font-bold text-error">-3</div>
<div class="h-1 w-full bg-surface-container-low rounded-full overflow-hidden">
<div class="h-full bg-error w-1/4"></div>
</div>
</div>
</div>
<div class="col-span-12 md:col-span-6">
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm flex items-center justify-between border border-outline-variant/10 relative overflow-hidden">
<div class="space-y-1 relative z-10">
<span class="text-xs font-bold uppercase tracking-widest text-on-surface-variant">Overall Risk Level</span>
<div class="flex items-center gap-3">
<h3 class="text-4xl font-bold text-amber-600">Moderate</h3>
<span class="bg-amber-100 text-amber-800 px-3 py-1 rounded-full text-xs font-bold">Action Needed</span>
</div>
</div>
<div class="relative z-10">
<span class="material-symbols-outlined text-6xl text-amber-500 opacity-40" data-icon="warning">warning</span>
</div>
<!-- Background Glow -->
<div class="absolute -right-10 -top-10 w-40 h-40 bg-amber-200/20 blur-3xl rounded-full"></div>
</div>
</div>
<!-- 2. Drift Timeline -->
<div class="col-span-12 lg:col-span-8">
<div class="bg-surface-container-lowest p-8 rounded-xl shadow-sm border border-outline-variant/10">
<div class="flex items-center justify-between mb-8">
<h3 class="headline-sm text-on-surface">Evolution Timeline</h3>
<div class="flex items-center gap-2 text-xs font-semibold text-on-surface-variant bg-surface-container-low px-3 py-1 rounded-full">
<span class="material-symbols-outlined text-sm" data-icon="history">history</span>
                                120 Days Tracking
                            </div>
</div>
<div class="relative py-12">
<!-- Timeline Line -->
<div class="absolute top-1/2 left-0 w-full h-0.5 bg-surface-container-high -translate-y-1/2"></div>
<div class="flex justify-between relative z-10">
<!-- Node 1 -->
<div class="flex flex-col items-center gap-4">
<div class="w-10 h-10 rounded-full bg-surface-container-highest flex items-center justify-center text-xs font-bold text-on-surface shadow-sm">v1.0.1</div>
<div class="text-center">
<p class="text-xs font-bold text-on-surface">Baseline</p>
<p class="text-[10px] text-on-surface-variant">Jan 12, 2024</p>
</div>
</div>
<!-- Node 2 -->
<div class="flex flex-col items-center gap-4">
<div class="w-4 h-4 rounded-full bg-surface-container-highest mt-3 shadow-sm"></div>
<div class="text-center">
<p class="text-xs font-semibold text-on-surface-variant">v1.0.2</p>
<p class="text-[10px] text-on-surface-variant">Feb 05</p>
</div>
</div>
<!-- Node 3 -->
<div class="flex flex-col items-center gap-4">
<div class="w-12 h-12 rounded-full bg-secondary-container flex items-center justify-center text-xs font-bold text-on-secondary-container shadow-md border-4 border-surface-container-lowest">v1.0.3</div>
<div class="text-center">
<p class="text-xs font-bold text-secondary">Major Patch</p>
<p class="text-[10px] text-on-surface-variant">Mar 18</p>
</div>
</div>
<!-- Node 4 (Current) -->
<div class="flex flex-col items-center gap-4">
<div class="w-14 h-14 rounded-full bg-primary flex items-center justify-center text-sm font-bold text-on-primary shadow-lg ring-4 ring-primary/20 ring-offset-2">v1.0.4</div>
<div class="text-center">
<p class="text-xs font-bold text-primary">Current</p>
<p class="text-[10px] text-on-surface-variant">Today</p>
</div>
</div>
</div>
</div>
</div>
</div>
<!-- 3. Drift Velocity Chart (Small) -->
<div class="col-span-12 lg:col-span-4">
<div class="bg-surface-container-lowest p-8 rounded-xl shadow-sm border border-outline-variant/10 h-full flex flex-col">
<h3 class="headline-sm text-on-surface mb-6">Drift Velocity</h3>
<div class="flex-grow flex items-end justify-between gap-2 px-2 pb-2">
<div class="w-full bg-surface-container-low rounded-t-lg h-12 group relative">
<div class="absolute bottom-full left-1/2 -translate-x-1/2 mb-2 bg-on-surface text-surface text-[10px] px-2 py-1 rounded opacity-0 group-hover:opacity-100 transition-opacity">4 chg</div>
</div>
<div class="w-full bg-surface-container-low rounded-t-lg h-24"></div>
<div class="w-full bg-primary-container rounded-t-lg h-40"></div>
<div class="w-full bg-surface-container-low rounded-t-lg h-16"></div>
<div class="w-full bg-primary rounded-t-lg h-56"></div>
<div class="w-full bg-primary-fixed-dim rounded-t-lg h-32"></div>
<div class="w-full bg-primary rounded-t-lg h-48"></div>
</div>
<div class="flex justify-between mt-4 text-[10px] font-bold text-on-surface-variant uppercase tracking-widest">
<span>Week 1</span>
<span>Week 4</span>
</div>
</div>
</div>
<!-- 4. Schema Diff Viewer -->
<div class="col-span-12 lg:col-span-8">
<div class="bg-[#1e293b] rounded-xl shadow-2xl overflow-hidden border border-slate-700">
<div class="bg-slate-800/50 px-6 py-4 border-b border-slate-700 flex justify-between items-center">
<div class="flex gap-2">
<div class="w-3 h-3 rounded-full bg-rose-500"></div>
<div class="w-3 h-3 rounded-full bg-amber-500"></div>
<div class="w-3 h-3 rounded-full bg-emerald-500"></div>
</div>
<span class="text-xs text-slate-400 font-mono">auth_service.schema.json</span>
<div class="flex items-center gap-4">
<span class="text-[10px] text-slate-500 font-bold uppercase tracking-widest">JSON Diff</span>
<span class="material-symbols-outlined text-slate-400 text-sm" data-icon="fullscreen">fullscreen</span>
</div>
</div>
<div class="p-6 code-font text-sm leading-relaxed overflow-x-auto">
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">12</span>
<span>{</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">13</span>
<span class="ml-4">"user_id": "string (uuid)",</span>
</div>
<div class="bg-red-900/30 text-rose-200 flex gap-4 -mx-6 px-6 border-l-4 border-rose-500">
<span class="w-6 shrink-0 text-rose-500/50">14</span>
<span class="ml-4">"legacy_id": "string", <span class="text-[10px] bg-rose-500/20 px-2 rounded-full uppercase tracking-widest font-sans font-bold ml-2">Deprecated</span></span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">15</span>
<span class="ml-4">"name": {</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">16</span>
<span class="ml-8">"first": "string",</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">17</span>
<span class="ml-8">"last": "string"</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">18</span>
<span class="ml-4">},</span>
</div>
<div class="bg-emerald-900/30 text-emerald-200 flex gap-4 -mx-6 px-6 border-l-4 border-emerald-500">
<span class="w-6 shrink-0 text-emerald-500/50">19</span>
<span class="ml-4">"accountStatus": "enum[active, trial, suspended]",</span>
</div>
<div class="bg-emerald-900/30 text-emerald-200 flex gap-4 -mx-6 px-6 border-l-4 border-emerald-500">
<span class="w-6 shrink-0 text-emerald-500/50">20</span>
<span class="ml-4">"mfa_enabled": "boolean",</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">21</span>
<span class="ml-4">"created_at": "timestamp"</span>
</div>
<div class="text-slate-500 flex gap-4">
<span class="w-6 shrink-0">22</span>
<span>}</span>
</div>
</div>
</div>
</div>
<!-- 5. Breaking Changes Panel -->
<div class="col-span-12 lg:col-span-4">
<div class="bg-surface-container-lowest rounded-xl shadow-sm border border-outline-variant/10 flex flex-col h-full overflow-hidden">
<div class="p-6 border-b border-outline-variant/5 flex items-center gap-3">
<span class="material-symbols-outlined text-error" data-icon="error_med">error_med</span>
<h3 class="title-md font-bold text-on-surface">Breaking Changes</h3>
</div>
<div class="flex-grow p-0">
<div class="divide-y divide-outline-variant/10">
<!-- Change 1 -->
<div class="p-6 hover:bg-surface-container-low transition-colors group">
<div class="flex items-start gap-4">
<div class="mt-1 p-2 bg-error/10 rounded-lg text-error">
<span class="material-symbols-outlined text-sm" data-icon="rule">rule</span>
</div>
<div class="space-y-1">
<p class="text-sm font-bold text-on-surface">Type Mismatch: accountStatus</p>
<p class="text-xs text-on-surface-variant leading-relaxed">Field changed from <code class="bg-surface-container-highest px-1 rounded">string</code> to <code class="bg-surface-container-highest px-1 rounded">enum</code>. Legacy clients may experience parsing failures.</p>
<div class="pt-2 flex gap-2">
<span class="text-[10px] font-bold bg-error text-on-error px-2 py-0.5 rounded-full uppercase">Critical</span>
<span class="text-[10px] font-bold text-primary uppercase tracking-tighter">Auth Service</span>
</div>
</div>
</div>
</div>
<!-- Change 2 -->
<div class="p-6 hover:bg-surface-container-low transition-colors group">
<div class="flex items-start gap-4">
<div class="mt-1 p-2 bg-amber-100 rounded-lg text-amber-600">
<span class="material-symbols-outlined text-sm" data-icon="remove_circle">remove_circle</span>
</div>
<div class="space-y-1">
<p class="text-sm font-bold text-on-surface">Deprecation: legacy_id</p>
<p class="text-xs text-on-surface-variant leading-relaxed">The field has been marked as deprecated and will be removed in v1.1.0. Migrate to <code class="bg-surface-container-highest px-1 rounded">user_id</code>.</p>
<div class="pt-2 flex gap-2">
<span class="text-[10px] font-bold bg-amber-500 text-white px-2 py-0.5 rounded-full uppercase">Warning</span>
<span class="text-[10px] font-bold text-primary uppercase tracking-tighter">Identity Core</span>
</div>
</div>
</div>
</div>
<!-- Change 3 -->
<div class="p-6 hover:bg-surface-container-low transition-colors group">
<div class="flex items-start gap-4">
<div class="mt-1 p-2 bg-emerald-100 rounded-lg text-emerald-600">
<span class="material-symbols-outlined text-sm" data-icon="info">info</span>
</div>
<div class="space-y-1">
<p class="text-sm font-bold text-on-surface">Required Param: mfa_enabled</p>
<p class="text-xs text-on-surface-variant leading-relaxed">New required field added to the base user profile. Default value set to <code class="bg-surface-container-highest px-1 rounded">false</code>.</p>
</div>
</div>
</div>
</div>
</div>
<div class="p-4 bg-surface-container-low text-center">
<button class="text-xs font-bold text-primary hover:underline">View All 17 Changes</button>
</div>
</div>
</div>
</div>
<!-- Footer Meta -->
<div class="flex justify-between items-center py-6 border-t border-outline-variant/10 text-on-surface-variant">
<div class="flex items-center gap-4 text-xs font-medium">
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-sm" data-icon="verified_user">verified_user</span> Verified Build</span>
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-sm" data-icon="sync">sync</span> Last Sync: 4 mins ago</span>
</div>
<div class="flex gap-6 text-[10px] font-bold uppercase tracking-widest">
<a class="hover:text-primary" href="#">Documentation</a>
<a class="hover:text-primary" href="#">API Reference</a>
<a class="hover:text-primary" href="#">Support</a>
</div>
</div>
</div>
</main>
</body></html>

<!-- Capture Inspector (Teal Clarity v2) -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>therAPI | Endpoint Explorer</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700&amp;family=Inter:wght@400;500;600&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    "colors": {
                        "tertiary-fixed-dim": "#bbc9c9",
                        "on-background": "#191c1d",
                        "on-error-container": "#93000a",
                        "secondary-container": "#a9ece5",
                        "surface-container": "#eceeee",
                        "tertiary": "#3f4d4d",
                        "on-tertiary": "#ffffff",
                        "on-primary-fixed": "#001f23",
                        "tertiary-fixed": "#d6e5e5",
                        "primary-fixed-dim": "#82d3de",
                        "inverse-primary": "#82d3de",
                        "tertiary-container": "#576565",
                        "on-tertiary-container": "#d3e2e2",
                        "surface-tint": "#006972",
                        "on-surface": "#191c1d",
                        "surface-container-low": "#f2f4f4",
                        "on-secondary-fixed-variant": "#00504b",
                        "on-primary-fixed-variant": "#004f56",
                        "background": "#f8fafa",
                        "secondary": "#236863",
                        "primary-fixed": "#9ff0fb",
                        "surface-bright": "#f8fafa",
                        "outline": "#6f797a",
                        "error": "#ba1a1a",
                        "secondary-fixed-dim": "#90d3cb",
                        "inverse-surface": "#2e3131",
                        "surface-container-highest": "#e1e3e3",
                        "surface-container-high": "#e6e8e9",
                        "on-primary-container": "#9becf7",
                        "primary": "#00535b",
                        "on-surface-variant": "#3e494a",
                        "on-secondary-fixed": "#00201e",
                        "surface-container-lowest": "#ffffff",
                        "primary-container": "#006d77",
                        "on-secondary": "#ffffff",
                        "on-error": "#ffffff",
                        "inverse-on-surface": "#eff1f1",
                        "error-container": "#ffdad6",
                        "surface-dim": "#d8dada",
                        "on-secondary-container": "#286d67",
                        "on-primary": "#ffffff",
                        "surface": "#f8fafa",
                        "on-tertiary-fixed-variant": "#3c494a",
                        "surface-variant": "#e1e3e3",
                        "secondary-fixed": "#acefe7",
                        "outline-variant": "#bec8ca",
                        "on-tertiary-fixed": "#101e1e"
                    },
                    "borderRadius": {
                        "DEFAULT": "0.25rem",
                        "lg": "0.5rem",
                        "xl": "0.75rem",
                        "full": "9999px"
                    },
                    "fontFamily": {
                        "headline": ["Manrope"],
                        "body": ["Inter"],
                        "label": ["Inter"]
                    }
                }
            }
        }
    </script>
<style>
        body { font-family: 'Inter', sans-serif; }
        h1, h2, h3, .font-manrope { font-family: 'Manrope', sans-serif; }
        .material-symbols-outlined {
            font-variation-settings: 'FILL' 0, 'wght' 400, 'GRAD' 0, 'opsz' 24;
            vertical-align: middle;
        }
        .sit-against { position: relative; }
        .glass-panel {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(20px);
        }
    </style>
</head>
<body class="bg-background text-on-surface">
<!-- SideNavBar -->
<aside class="h-screen w-64 fixed left-0 top-0 border-r-0 bg-slate-50 dark:bg-slate-900 flex flex-col py-8 px-4 font-manrope text-sm font-medium z-50">
<div class="mb-10 px-2">
<h1 class="text-2xl font-bold text-[#006D77] tracking-tight">therAPI</h1>
<p class="text-[10px] uppercase tracking-widest text-on-surface-variant/60 font-bold mt-1">Clinical API Sanctuary</p>
</div>
<nav class="flex-1 space-y-1">
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-slate-500 dark:text-slate-400 hover:text-[#006D77] hover:bg-slate-100 transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="dashboard">dashboard</span>
<span>Control Panel</span>
</a>
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-[#006D77] font-bold border-r-4 border-[#006D77] bg-[#006D77]/5 transition-all duration-200" href="#">
<span class="material-symbols-outlined" data-icon="explore">explore</span>
<span>Explorer</span>
</a>
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-slate-500 dark:text-slate-400 hover:text-[#006D77] hover:bg-slate-100 transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="query_stats">query_stats</span>
<span>Drift</span>
</a>
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-slate-500 dark:text-slate-400 hover:text-[#006D77] hover:bg-slate-100 transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="troubleshoot">troubleshoot</span>
<span>Inspector</span>
</a>
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-slate-500 dark:text-slate-400 hover:text-[#006D77] hover:bg-slate-100 transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="ios_share">ios_share</span>
<span>Export</span>
</a>
<a class="flex items-center gap-3 px-3 py-2.5 rounded-xl text-slate-500 dark:text-slate-400 hover:text-[#006D77] hover:bg-slate-100 transition-colors" href="#">
<span class="material-symbols-outlined" data-icon="settings">settings</span>
<span>Settings</span>
</a>
</nav>
<div class="mt-auto px-2 flex items-center gap-3">
<div class="w-10 h-10 rounded-full overflow-hidden bg-surface-container">
<img class="w-full h-full object-cover" data-alt="professional clinical portrait of a female doctor in a white coat against a soft neutral background" src="https://lh3.googleusercontent.com/aida-public/AB6AXuDOrz3l8bb4be1wTqyvyihd_JqimSiyF64ogN2tRohzRX7b4ageEm6JpJEjNQxO2loHrl-jR7MOqr5zFZiQMV5JoFZ_sZZoTxjsNdy282-Ccw3jGrZstwVf5zmnrbys9rF8knJtXW6VGsqSZXnkskFN3MXk7hVBAySjEMZAmkhfiK0WNVdXu7wvgX8wBfykT9cAIFgXGG696D_nkr_zpfuYZD4vqqTjVQAz18a55BXZkikiF6StS8ZP1wSN2WFhx_zBt9rX7l6rW2A"/>
</div>
<div>
<p class="text-xs font-bold text-on-surface">Dr. Aris Thorne</p>
<p class="text-[10px] text-on-surface-variant">Lead Architect</p>
</div>
</div>
</aside>
<!-- Main Content Area -->
<main class="ml-64 min-h-screen">
<!-- TopNavBar -->
<header class="fixed top-0 right-0 w-[calc(100%-16rem)] h-16 bg-white/85 dark:bg-slate-950/85 backdrop-blur-md border-b border-slate-100/15 flex justify-between items-center px-8 z-40 font-inter text-sm shadow-sm dark:shadow-none">
<div class="flex items-center gap-8">
<div class="flex items-center gap-2 bg-surface-container-low px-4 py-2 rounded-full">
<span class="material-symbols-outlined text-outline text-lg" data-icon="search">search</span>
<input class="bg-transparent border-none focus:ring-0 text-sm w-64" placeholder="Search commands or endpoints..." type="text"/>
</div>
<div class="flex items-center gap-6">
<a class="text-[#006D77] font-semibold hover:text-[#006D77] transition-all" href="#">Connected</a>
<a class="text-slate-500 dark:text-slate-400 hover:text-[#006D77] transition-all" href="#">Production</a>
</div>
</div>
<div class="flex items-center gap-4">
<button class="bg-primary text-white px-5 py-2 rounded-xl text-xs font-semibold flex items-center gap-2 hover:bg-primary-container transition-all">
                    Environment
                    <span class="material-symbols-outlined text-sm" data-icon="expand_more">expand_more</span>
</button>
<button class="text-outline hover:text-primary transition-colors">
<span class="material-symbols-outlined text-2xl" data-icon="account_circle">account_circle</span>
</button>
</div>
</header>
<!-- Content Canvas -->
<div class="pt-24 pb-12 px-8 flex gap-6">
<!-- Left Sidebar Filter -->
<div class="w-80 flex flex-col gap-6">
<div class="bg-surface-container-lowest rounded-xl p-6 shadow-sm">
<h3 class="text-sm font-bold font-manrope text-on-surface mb-4">Filters</h3>
<div class="space-y-6">
<div>
<label class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant block mb-2">Method</label>
<div class="grid grid-cols-2 gap-2">
<button class="px-3 py-2 rounded-lg bg-primary text-white text-xs font-bold">ALL</button>
<button class="px-3 py-2 rounded-lg bg-surface-container text-on-surface-variant text-xs font-bold hover:bg-surface-container-high transition-colors">GET</button>
<button class="px-3 py-2 rounded-lg bg-surface-container text-on-surface-variant text-xs font-bold hover:bg-surface-container-high transition-colors">POST</button>
<button class="px-3 py-2 rounded-lg bg-surface-container text-on-surface-variant text-xs font-bold hover:bg-surface-container-high transition-colors">PUT</button>
</div>
</div>
<div class="flex items-center justify-between">
<label class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant">Changed Only</label>
<button class="w-10 h-5 bg-surface-dim rounded-full relative transition-colors">
<div class="absolute left-0.5 top-0.5 w-4 h-4 bg-white rounded-full shadow-sm"></div>
</button>
</div>
</div>
</div>
<!-- Endpoint List -->
<div class="bg-surface-container-lowest rounded-xl overflow-hidden shadow-sm">
<div class="p-4 border-b border-surface-container">
<p class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant">Endpoints (14)</p>
</div>
<div class="divide-y divide-surface-container/30">
<div class="p-4 bg-primary/5 border-l-4 border-primary cursor-pointer transition-all">
<div class="flex items-center justify-between mb-1">
<span class="px-2 py-0.5 rounded text-[9px] font-extrabold bg-[#006D77]/10 text-[#006D77]">GET</span>
<span class="px-2 py-0.5 rounded-full text-[9px] font-bold bg-green-100 text-green-700">DRIFT LOW</span>
</div>
<p class="text-xs font-mono font-medium text-on-surface truncate">/api/v1/user/profile</p>
</div>
<div class="p-4 hover:bg-surface-container-low cursor-pointer transition-all">
<div class="flex items-center justify-between mb-1">
<span class="px-2 py-0.5 rounded text-[9px] font-extrabold bg-blue-100 text-blue-700">POST</span>
<span class="px-2 py-0.5 rounded-full text-[9px] font-bold bg-amber-100 text-amber-700">DRIFT MOD</span>
</div>
<p class="text-xs font-mono font-medium text-on-surface truncate">/api/v1/auth/session</p>
</div>
<div class="p-4 hover:bg-surface-container-low cursor-pointer transition-all">
<div class="flex items-center justify-between mb-1">
<span class="px-2 py-0.5 rounded text-[9px] font-extrabold bg-[#006D77]/10 text-[#006D77]">GET</span>
<span class="px-2 py-0.5 rounded-full text-[9px] font-bold bg-green-100 text-green-700">DRIFT LOW</span>
</div>
<p class="text-xs font-mono font-medium text-on-surface truncate">/api/v1/clinical/vitals</p>
</div>
<div class="p-4 hover:bg-surface-container-low cursor-pointer transition-all">
<div class="flex items-center justify-between mb-1">
<span class="px-2 py-0.5 rounded text-[9px] font-extrabold bg-blue-100 text-blue-700">POST</span>
<span class="px-2 py-0.5 rounded-full text-[9px] font-bold bg-red-100 text-red-700">DRIFT HIGH</span>
</div>
<p class="text-xs font-mono font-medium text-on-surface truncate">/api/v1/patient/onboard</p>
</div>
</div>
</div>
</div>
<!-- Endpoint Detail Column -->
<div class="flex-1 space-y-6">
<!-- Hero Header -->
<div class="bg-surface-container-lowest rounded-xl p-8 shadow-sm relative overflow-hidden">
<div class="absolute top-0 right-0 w-48 h-48 bg-primary/5 rounded-full -mr-12 -mt-12"></div>
<div class="relative z-10">
<div class="flex items-center gap-3 mb-2">
<span class="px-3 py-1 rounded text-xs font-extrabold bg-[#006D77] text-white">GET</span>
<h2 class="text-2xl font-bold font-manrope text-on-surface">/api/v1/user/profile</h2>
</div>
<p class="text-on-surface-variant text-sm">Retrieves core clinician profile data, licensing status, and department associations.</p>
</div>
</div>
<!-- Stats Bento Grid -->
<div class="grid grid-cols-4 gap-4">
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm border-b-2 border-primary/20">
<p class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant mb-1">Success Rate</p>
<p class="text-3xl font-bold font-manrope text-primary">99.8%</p>
<div class="mt-2 w-full bg-surface-container h-1 rounded-full overflow-hidden">
<div class="bg-primary h-full" style="width: 99.8%"></div>
</div>
</div>
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm border-b-2 border-primary/20">
<p class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant mb-1">Avg Latency</p>
<p class="text-3xl font-bold font-manrope text-on-surface">42<span class="text-sm ml-1 font-medium text-outline">ms</span></p>
<p class="text-[10px] text-green-600 font-bold mt-2">? 4% vs last week</p>
</div>
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm border-b-2 border-primary/20">
<p class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant mb-1">Daily Hits</p>
<p class="text-3xl font-bold font-manrope text-on-surface">1.2<span class="text-sm ml-1 font-medium text-outline">M</span></p>
<p class="text-[10px] text-on-surface-variant mt-2">+12k peak concurrent</p>
</div>
<div class="bg-surface-container-lowest p-6 rounded-xl shadow-sm border-b-2 border-primary/20">
<p class="text-[10px] font-bold uppercase tracking-widest text-on-surface-variant mb-1">Drift Risk</p>
<div class="flex items-center gap-2">
<span class="w-3 h-3 rounded-full bg-green-500"></span>
<p class="text-3xl font-bold font-manrope text-green-600">LOW</p>
</div>
<p class="text-[10px] text-on-surface-variant mt-2">Last checked 2m ago</p>
</div>
</div>
<!-- Tabs & Content -->
<div class="bg-surface-container-lowest rounded-xl shadow-sm overflow-hidden">
<div class="flex border-b border-surface-container">
<button class="px-8 py-4 text-sm font-bold text-primary border-b-2 border-primary">Summary</button>
<button class="px-8 py-4 text-sm font-medium text-outline hover:text-on-surface transition-colors">Schema Versions</button>
<button class="px-8 py-4 text-sm font-medium text-outline hover:text-on-surface transition-colors">Captures</button>
<button class="px-8 py-4 text-sm font-medium text-outline hover:text-on-surface transition-colors">OpenAPI</button>
</div>
<div class="p-8 space-y-10">
<!-- Headers Section -->
<section>
<h3 class="text-sm font-bold font-manrope text-on-surface mb-4 flex items-center gap-2">
<span class="material-symbols-outlined text-primary text-lg" data-icon="list_alt">list_alt</span>
                                Observed Request Headers
                            </h3>
<div class="space-y-3">
<div class="flex items-center justify-between p-3 rounded-lg bg-surface-container-low border border-transparent hover:border-outline-variant/30 transition-all">
<div class="flex items-center gap-4">
<code class="text-xs font-bold text-primary">Authorization</code>
<span class="text-[10px] px-2 py-0.5 rounded-full bg-secondary-container/30 text-secondary font-bold">REQUIRED</span>
</div>
<span class="text-xs text-on-surface-variant font-mono">Bearer &lt;JWT&gt;</span>
</div>
<div class="flex items-center justify-between p-3 rounded-lg bg-surface-container-low border border-transparent hover:border-outline-variant/30 transition-all">
<div class="flex items-center gap-4">
<code class="text-xs font-bold text-primary">X-Practitioner-ID</code>
<span class="text-[10px] px-2 py-0.5 rounded-full bg-secondary-container/30 text-secondary font-bold">REQUIRED</span>
</div>
<span class="text-xs text-on-surface-variant font-mono">UUID v4</span>
</div>
<div class="flex items-center justify-between p-3 rounded-lg bg-surface-container-low border border-transparent hover:border-outline-variant/30 transition-all">
<div class="flex items-center gap-4">
<code class="text-xs font-bold text-primary">Accept-Language</code>
<span class="text-[10px] px-2 py-0.5 rounded-full bg-surface-container text-outline font-bold">OPTIONAL</span>
</div>
<span class="text-xs text-on-surface-variant font-mono">en-US, es-MX</span>
</div>
</div>
</section>
<!-- Evolution Timeline -->
<section>
<h3 class="text-sm font-bold font-manrope text-on-surface mb-6 flex items-center gap-2">
<span class="material-symbols-outlined text-primary text-lg" data-icon="history">history</span>
                                Version Evolution
                            </h3>
<div class="relative pl-8 border-l-2 border-surface-container space-y-8">
<div class="relative">
<div class="absolute -left-[41px] top-0 w-4 h-4 rounded-full bg-primary border-4 border-white"></div>
<div class="flex items-center justify-between mb-1">
<h4 class="text-sm font-bold text-on-surface">v1.4.2 — Latest stable</h4>
<span class="text-[10px] text-outline font-bold">OCT 24, 2023</span>
</div>
<p class="text-xs text-on-surface-variant">Added <code class="bg-surface-container px-1 rounded">department_code</code> to root response schema.</p>
</div>
<div class="relative">
<div class="absolute -left-[41px] top-0 w-4 h-4 rounded-full bg-outline-variant border-4 border-white"></div>
<div class="flex items-center justify-between mb-1">
<h4 class="text-sm font-bold text-on-surface-variant">v1.4.0</h4>
<span class="text-[10px] text-outline font-bold">SEP 12, 2023</span>
</div>
<p class="text-xs text-on-surface-variant">Performance optimization for multi-tenant licensing lookups.</p>
</div>
<div class="relative">
<div class="absolute -left-[41px] top-0 w-4 h-4 rounded-full bg-outline-variant border-4 border-white"></div>
<div class="flex items-center justify-between mb-1">
<h4 class="text-sm font-bold text-on-surface-variant">v1.3.9 — Initial Release</h4>
<span class="text-[10px] text-outline font-bold">AUG 01, 2023</span>
</div>
<p class="text-xs text-on-surface-variant">Baseline endpoint architecture established.</p>
</div>
</div>
</section>
</div>
</div>
</div>
</div>
</main>
<!-- Floating Vitality Glass Card (Status Summary) -->
<div class="fixed bottom-8 right-8 w-64 glass-panel rounded-xl p-4 shadow-2xl border border-white/20 z-50">
<div class="flex items-center justify-between mb-4">
<span class="text-[10px] font-bold uppercase tracking-widest text-primary">System Vitality</span>
<span class="w-2 h-2 rounded-full bg-green-500 animate-pulse"></span>
</div>
<div class="space-y-3">
<div class="flex items-center justify-between">
<span class="text-xs text-on-surface-variant">Global Drift</span>
<span class="text-xs font-bold text-on-surface">0.02%</span>
</div>
<div class="flex items-center justify-between">
<span class="text-xs text-on-surface-variant">API Health</span>
<span class="text-xs font-bold text-on-surface">Optimal</span>
</div>
<div class="pt-2 mt-2 border-t border-surface-container/50">
<button class="w-full py-2 bg-primary text-white rounded-lg text-xs font-bold hover:bg-primary-container transition-all">
                    Generate Report
                </button>
</div>
</div>
<!-- Gradient Glow -->
<div class="absolute top-0 right-0 w-12 h-12 bg-primary/20 blur-2xl -mr-6 -mt-6"></div>
</div>
</body></html>

<!-- Schema Drift (therAPI) -->
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>therAPI | Schema Drift Analysis</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
      tailwind.config = {
        darkMode: "class",
        theme: {
          extend: {
            "colors": {
                    "surface-container": "#edeeee",
                    "error": "#ba1a1a",
                    "primary-container": "#005b63",
                    "on-surface": "#191c1c",
                    "tertiary": "#004247",
                    "on-tertiary-container": "#84d2db",
                    "inverse-surface": "#2e3131",
                    "surface-tint": "#1a6870",
                    "surface-bright": "#f8f9f9",
                    "inverse-on-surface": "#f0f1f1",
                    "on-primary": "#ffffff",
                    "primary": "#004248",
                    "secondary": "#505f78",
                    "on-primary-fixed-variant": "#004f56",
                    "on-surface-variant": "#3f484a",
                    "on-tertiary-fixed": "#002023",
                    "secondary-fixed-dim": "#b8c7e4",
                    "on-secondary-container": "#54637d",
                    "on-tertiary": "#ffffff",
                    "background": "#f8f9f9",
                    "on-tertiary-fixed-variant": "#004f55",
                    "on-secondary-fixed": "#0c1c32",
                    "error-container": "#ffdad6",
                    "surface-container-highest": "#e1e3e3",
                    "on-primary-container": "#8cd0d9",
                    "surface-container-high": "#e7e8e8",
                    "surface-dim": "#d9dada",
                    "primary-fixed-dim": "#8dd2db",
                    "on-secondary": "#ffffff",
                    "inverse-primary": "#8dd2db",
                    "surface-container-lowest": "#ffffff",
                    "outline": "#6f797a",
                    "tertiary-container": "#005b62",
                    "on-error-container": "#93000a",
                    "on-background": "#191c1c",
                    "secondary-container": "#d1e0fe",
                    "surface-container-low": "#f3f4f4",
                    "on-primary-fixed": "#001f23",
                    "tertiary-fixed": "#a1eff9",
                    "on-error": "#ffffff",
                    "surface": "#f8f9f9",
                    "surface-variant": "#e1e3e3",
                    "primary-fixed": "#a9eef7",
                    "secondary-fixed": "#d5e3ff",
                    "tertiary-fixed-dim": "#85d3dc",
                    "on-secondary-fixed-variant": "#394760",
                    "outline-variant": "#bec8ca"
            },
            "borderRadius": {
                    "DEFAULT": "0.125rem",
                    "lg": "0.25rem",
                    "xl": "0.5rem",
                    "full": "0.75rem"
            },
            "fontFamily": {
                    "headline": ["Inter"],
                    "body": ["Inter"],
                    "label": ["Inter"]
            }
          },
        },
      }
    </script>
<style>
        body { font-family: 'Inter', sans-serif; background-color: #F3F4F4; }
        .material-symbols-outlined { font-variation-settings: 'FILL' 0, 'wght' 300, 'GRAD' 0, 'opsz' 24; }
        .signature-gradient { background: linear-gradient(135deg, #005B63 0%, #7FCDD6 100%); }
        .glass-panel { background: rgba(255, 255, 255, 0.85); backdrop-filter: blur(12px); }
        .code-bg { background-color: #1B2740; }
        .code-added { background-color: #0E5E57; }
        .code-removed { background-color: #6C2D35; }
        .ambient-shadow { box-shadow: 0 12px 32px -4px rgba(32, 36, 38, 0.08); }
        .ghost-border { border: 1px solid rgba(231, 232, 232, 0.4); }
    </style>
</head>
<body class="text-on-surface selection:bg-primary-fixed selection:text-on-primary-fixed">
<!-- SideNavBar Anchor -->
<aside class="bg-[#FAFAFA] dark:bg-slate-900 h-screen w-64 fixed left-0 top-0 flex flex-col py-6 font-inter text-sm font-medium tracking-tight">
<div class="px-6 mb-10 flex items-center gap-3">
<div class="w-8 h-8 signature-gradient rounded-lg flex items-center justify-center">
<span class="material-symbols-outlined text-white text-lg" style="font-variation-settings: 'FILL' 1;">api</span>
</div>
<div>
<h1 class="text-xl font-bold text-[#005B63] dark:text-[#7FCDD6] tracking-tighter">therAPI</h1>
<p class="text-[10px] uppercase tracking-widest text-slate-400">API Orchestration</p>
</div>
</div>
<nav class="flex-1 px-4 space-y-1">
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 hover:bg-slate-100 transition-colors duration-200" href="#">
<span class="material-symbols-outlined">dashboard</span> Control Panel
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 hover:bg-slate-100 transition-colors duration-200" href="#">
<span class="material-symbols-outlined">explore</span> Explorer
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-[#005B63] font-bold border-r-4 border-[#005B63] bg-[#005B63]/5" href="#">
<span class="material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">compare_arrows</span> Drift
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 hover:bg-slate-100 transition-colors duration-200" href="#">
<span class="material-symbols-outlined">search_check</span> Inspector
            </a>
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 hover:bg-slate-100 transition-colors duration-200" href="#">
<span class="material-symbols-outlined">download</span> Export
            </a>
<div class="pt-6 mt-6 border-t border-slate-100">
<a class="flex items-center gap-3 px-4 py-3 rounded-lg text-slate-500 hover:bg-slate-100 transition-colors duration-200" href="#">
<span class="material-symbols-outlined">settings</span> Settings
                </a>
</div>
</nav>
</aside>
<!-- TopNavBar Anchor -->
<header class="fixed top-0 right-0 left-64 h-16 z-40 bg-white/85 backdrop-blur-md flex items-center justify-between px-8 shadow-sm">
<div class="flex items-center gap-4 flex-1">
<div class="relative w-full max-w-md">
<span class="material-symbols-outlined absolute left-3 top-1/2 -translate-y-1/2 text-slate-400 text-sm">search</span>
<input class="w-full pl-10 pr-4 py-2 bg-surface-container-low rounded-full border-none text-sm focus:ring-2 focus:ring-primary-container/20" placeholder="Search schema versions..." type="text"/>
</div>
</div>
<div class="flex items-center gap-6">
<div class="flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span>
<span class="text-xs font-semibold text-slate-500">Connected</span>
</div>
<div class="h-4 w-px bg-slate-200"></div>
<div class="flex items-center gap-2">
<span class="text-xs font-bold text-[#005B63]">Production</span>
<span class="material-symbols-outlined text-slate-400">account_circle</span>
</div>
</div>
</header>
<!-- Main Content Stage -->
<main class="pl-64 pt-16 min-h-screen">
<div class="p-10 max-w-7xl mx-auto">
<!-- Comparison Header -->
<header class="mb-10 flex justify-between items-end">
<div>
<h2 class="text-[2.75rem] font-extrabold tracking-tighter text-primary leading-tight mb-2">Schema Drift Analysis</h2>
<div class="flex items-center gap-3">
<span class="px-3 py-1 bg-surface-container-highest text-slate-600 rounded-lg text-xs font-bold">v1.0.1</span>
<span class="material-symbols-outlined text-slate-300">east</span>
<span class="px-3 py-1 bg-primary-container text-on-primary-container rounded-lg text-xs font-bold">v1.0.4 (Current)</span>
</div>
</div>
<div class="flex gap-4">
<button class="px-5 py-2.5 rounded-xl text-primary font-bold text-sm hover:bg-primary/5 transition-colors">
                        Download Report
                    </button>
<button class="px-6 py-2.5 rounded-xl signature-gradient text-white font-bold text-sm shadow-lg shadow-primary-container/20">
                        Approve Changes
                    </button>
</div>
</header>
<!-- Top Stats - Bento Grid Pattern -->
<div class="grid grid-cols-1 md:grid-cols-4 gap-6 mb-12">
<div class="bg-surface-container-lowest p-6 rounded-2xl ambient-shadow">
<p class="text-[0.75rem] font-medium text-slate-500 tracking-wider uppercase mb-1">Fields Added</p>
<div class="flex items-baseline gap-2">
<span class="text-3xl font-extrabold text-emerald-600">+14</span>
<span class="text-xs text-slate-400">new entries</span>
</div>
</div>
<div class="bg-surface-container-lowest p-6 rounded-2xl ambient-shadow">
<p class="text-[0.75rem] font-medium text-slate-500 tracking-wider uppercase mb-1">Fields Removed</p>
<div class="flex items-baseline gap-2">
<span class="text-3xl font-extrabold text-error">-3</span>
<span class="text-xs text-slate-400">deleted</span>
</div>
</div>
<div class="bg-surface-container-lowest p-6 rounded-2xl ambient-shadow border-l-4 border-[#FFB020]">
<p class="text-[0.75rem] font-medium text-slate-500 tracking-wider uppercase mb-1">Risk Level</p>
<div class="flex items-baseline gap-2">
<span class="text-3xl font-extrabold text-[#FFB020]">MODERATE</span>
</div>
</div>
<div class="bg-surface-container-lowest p-6 rounded-2xl ambient-shadow">
<p class="text-[0.75rem] font-medium text-slate-500 tracking-wider uppercase mb-1">Total Endpoints</p>
<div class="flex items-baseline gap-2">
<span class="text-3xl font-extrabold text-primary">142</span>
<span class="text-xs text-slate-400">monitored</span>
</div>
</div>
</div>
<!-- Asymmetric Layout: Evolution & Charts -->
<div class="grid grid-cols-12 gap-10 mb-12">
<!-- Evolution Timeline (Column 1-4) -->
<div class="col-span-12 lg:col-span-4 space-y-6">
<h3 class="text-lg font-bold text-primary px-2">Evolution Timeline</h3>
<div class="bg-surface-container-lowest p-8 rounded-2xl ghost-border space-y-8">
<div class="relative pl-8 border-l-2 border-surface-container-highest">
<div class="absolute -left-[9px] top-0 w-4 h-4 rounded-full border-4 border-white signature-gradient"></div>
<p class="text-xs font-bold text-primary">JULY 2024</p>
<p class="text-sm font-semibold text-on-surface">v1.0.4 Released</p>
<p class="text-xs text-slate-500">Stability improvements &amp; Auth patches</p>
</div>
<div class="relative pl-8 border-l-2 border-surface-container-highest">
<div class="absolute -left-[9px] top-0 w-4 h-4 rounded-full border-4 border-white bg-slate-300"></div>
<p class="text-xs font-bold text-slate-400">MAY 2024</p>
<p class="text-sm font-semibold text-on-surface">v1.0.2 Patch</p>
<p class="text-xs text-slate-500">Minor schema optimization</p>
</div>
<div class="relative pl-8 border-l-2 border-surface-container-highest">
<div class="absolute -left-[9px] top-0 w-4 h-4 rounded-full border-4 border-white bg-slate-300"></div>
<p class="text-xs font-bold text-slate-400">MARCH 2024</p>
<p class="text-sm font-semibold text-on-surface">v1.0.1 Baseline</p>
<p class="text-xs text-slate-500">Initial production deployment</p>
</div>
</div>
</div>
<!-- Drift Velocity Chart (Column 5-12) -->
<div class="col-span-12 lg:col-span-8 space-y-6">
<h3 class="text-lg font-bold text-primary px-2">Drift Velocity</h3>
<div class="bg-surface-container-lowest p-8 rounded-2xl ghost-border h-full min-h-[320px] flex flex-col">
<div class="flex-1 flex items-end gap-6 px-4">
<!-- Bars representing drift over time -->
<div class="flex-1 flex flex-col items-center gap-2 group">
<div class="w-full bg-surface-container-highest rounded-t-lg h-24 group-hover:bg-primary-fixed-dim transition-colors duration-300"></div>
<span class="text-[10px] font-bold text-slate-400 uppercase">Mar</span>
</div>
<div class="flex-1 flex flex-col items-center gap-2 group">
<div class="w-full bg-surface-container-highest rounded-t-lg h-32 group-hover:bg-primary-fixed-dim transition-colors duration-300"></div>
<span class="text-[10px] font-bold text-slate-400 uppercase">Apr</span>
</div>
<div class="flex-1 flex flex-col items-center gap-2 group">
<div class="w-full bg-surface-container-highest rounded-t-lg h-48 group-hover:bg-primary-fixed-dim transition-colors duration-300"></div>
<span class="text-[10px] font-bold text-slate-400 uppercase">May</span>
</div>
<div class="flex-1 flex flex-col items-center gap-2 group">
<div class="w-full bg-surface-container-highest rounded-t-lg h-16 group-hover:bg-primary-fixed-dim transition-colors duration-300"></div>
<span class="text-[10px] font-bold text-slate-400 uppercase">Jun</span>
</div>
<div class="flex-1 flex flex-col items-center gap-2 group">
<div class="w-full signature-gradient rounded-t-lg h-64 shadow-xl shadow-primary-container/10"></div>
<span class="text-[10px] font-bold text-primary uppercase">Jul</span>
</div>
</div>
<div class="mt-8 pt-6 border-t border-slate-50 flex justify-between items-center">
<div class="flex items-center gap-6">
<div class="flex items-center gap-2">
<span class="w-2 h-2 rounded-full signature-gradient"></span>
<span class="text-xs text-slate-500">Major Changes</span>
</div>
<div class="flex items-center gap-2">
<span class="w-2 h-2 rounded-full bg-surface-container-highest"></span>
<span class="text-xs text-slate-500">Minor Fixes</span>
</div>
</div>
<p class="text-xs font-medium text-slate-400 italic">Data updated 2m ago</p>
</div>
</div>
</div>
</div>
<!-- Code Diff & Breaking Changes List -->
<div class="grid grid-cols-1 lg:grid-cols-2 gap-10">
<!-- Code Diff Viewer -->
<div class="space-y-6">
<div class="flex items-center justify-between px-2">
<h3 class="text-lg font-bold text-primary">Schema Diff</h3>
<span class="text-[10px] font-mono bg-primary-container/10 text-primary-container px-2 py-1 rounded">JSON (RFC 8259)</span>
</div>
<div class="code-bg rounded-2xl overflow-hidden ambient-shadow font-mono text-sm leading-relaxed text-[#DDE6EE]">
<div class="flex bg-slate-800/50 px-4 py-2 border-b border-white/5 items-center gap-2">
<div class="w-3 h-3 rounded-full bg-error/40"></div>
<div class="w-3 h-3 rounded-full bg-[#FFB020]/40"></div>
<div class="w-3 h-3 rounded-full bg-emerald-500/40"></div>
<span class="text-xs text-slate-400 ml-4">user_schema_v1.0.4.json</span>
</div>
<div class="p-6">
<div class="flex">
<span class="w-8 opacity-30 select-none">1</span>
<span>{</span>
</div>
<div class="flex">
<span class="w-8 opacity-30 select-none">2</span>
<span class="ml-4 text-slate-400">"user_id": "uuid",</span>
</div>
<div class="flex code-removed w-full">
<span class="w-8 opacity-30 select-none">3</span>
<span class="ml-4">- "legacy_token": "string",</span>
</div>
<div class="flex code-added w-full">
<span class="w-8 opacity-30 select-none">4</span>
<span class="ml-4">+ "auth_provider": "enum[GOOGLE, GITHUB, APPLE]",</span>
</div>
<div class="flex code-added w-full">
<span class="w-8 opacity-30 select-none">5</span>
<span class="ml-4">+ "mfa_enabled": "boolean",</span>
</div>
<div class="flex">
<span class="w-8 opacity-30 select-none">6</span>
<span class="ml-4">"metadata": {</span>
</div>
<div class="flex">
<span class="w-8 opacity-30 select-none">7</span>
<span class="ml-8 text-slate-400">"last_login": "timestamp"</span>
</div>
<div class="flex">
<span class="w-8 opacity-30 select-none">8</span>
<span class="ml-4">}</span>
</div>
<div class="flex">
<span class="w-8 opacity-30 select-none">9</span>
<span>}</span>
</div>
</div>
</div>
</div>
<!-- Breaking Changes List -->
<div class="space-y-6">
<h3 class="text-lg font-bold text-primary px-2">Identified Risks</h3>
<div class="space-y-4">
<!-- Risk Card 1 -->
<div class="bg-surface-container-lowest p-6 rounded-2xl ghost-border flex items-start gap-4 group hover:bg-white transition-all">
<div class="p-3 bg-error-container text-error rounded-xl">
<span class="material-symbols-outlined">warning</span>
</div>
<div class="flex-1">
<div class="flex justify-between items-center mb-1">
<h4 class="font-bold text-on-surface">Type Mismatch: legacy_id</h4>
<span class="text-[10px] font-bold px-2 py-0.5 rounded-full bg-error/10 text-error uppercase">Critical</span>
</div>
<p class="text-sm text-slate-500 mb-3">Field changed from <code class="bg-slate-100 px-1 rounded">Integer</code> to <code class="bg-slate-100 px-1 rounded">String</code>. This will break existing downstream integrations.</p>
<div class="flex gap-2">
<span class="text-[10px] font-medium text-primary bg-primary/5 px-2 py-1 rounded">Auth Module</span>
<span class="text-[10px] font-medium text-primary bg-primary/5 px-2 py-1 rounded">v1.0.4 Regression</span>
</div>
</div>
</div>
<!-- Risk Card 2 -->
<div class="bg-surface-container-lowest p-6 rounded-2xl ghost-border flex items-start gap-4 group hover:bg-white transition-all">
<div class="p-3 bg-secondary-container text-secondary rounded-xl">
<span class="material-symbols-outlined">history</span>
</div>
<div class="flex-1">
<div class="flex justify-between items-center mb-1">
<h4 class="font-bold text-on-surface">Deprecation: /api/v1/user/tokens</h4>
<span class="text-[10px] font-bold px-2 py-0.5 rounded-full bg-secondary-container text-secondary uppercase">Notice</span>
</div>
<p class="text-sm text-slate-500 mb-3">Endpoint marked as deprecated. Migration suggested to <code class="bg-slate-100 px-1 rounded">/api/v2/auth/sessions</code> before 2025.</p>
<div class="flex gap-2">
<span class="text-[10px] font-medium text-primary bg-primary/5 px-2 py-1 rounded">Global API</span>
</div>
</div>
</div>
<!-- Risk Card 3 -->
<div class="bg-surface-container-lowest p-6 rounded-2xl ghost-border flex items-start gap-4 group hover:bg-white transition-all">
<div class="p-3 bg-primary-container/10 text-primary-container rounded-xl">
<span class="material-symbols-outlined">rule</span>
</div>
<div class="flex-1">
<div class="flex justify-between items-center mb-1">
<h4 class="font-bold text-on-surface">Missing Validation: phone_no</h4>
<span class="text-[10px] font-bold px-2 py-0.5 rounded-full bg-surface-container-highest text-slate-500 uppercase">Warning</span>
</div>
<p class="text-sm text-slate-500 mb-3">Newly added field lacks a defined regex pattern. Potential data integrity issue.</p>
<div class="flex gap-2">
<span class="text-[10px] font-medium text-primary bg-primary/5 px-2 py-1 rounded">User Profile</span>
</div>
</div>
</div>
</div>
</div>
</div>
<!-- Footer Documentation Link -->
<footer class="mt-20 pt-10 border-t border-slate-200 flex flex-col md:flex-row gap-8 items-center justify-between">
<div class="flex items-center gap-6">
<img alt="therAPI logo" class="h-6 opacity-20" data-alt="minimal monochrome logo of an abstract digital link symbol in light grey" src="https://lh3.googleusercontent.com/aida-public/AB6AXuA2pXCKN8SS7Xoe0a5miFCtALg3lL_WUDzy8tOMmfpsWlTSF34ySZXBJ2YnuPcukNBXOJlU1zK9HywbecpwyfQaxUADM-kIw77fv2w7vdomxJ-IXPb4xDSFj2uB6bkaDuXwklD1Zi2acsXqlTK39cyQQgMNUSHHA65-8-x_OaiJlku1L0NLvel8Qo7JZCXq9WXZ0Dlb8L_i9b8-t9ABTngIMhmm5FtfKyf_u-yA8uskODZKHfU7zYw60Q78YpKGiqdX1nqzaHlRaCA"/>
<p class="text-xs text-slate-400 font-medium tracking-wide">© 2024 therAPI Orchestration System. High-fidelity schema monitoring.</p>
</div>
<div class="flex gap-8">
<a class="text-xs font-bold text-primary hover:underline decoration-2 underline-offset-4" href="#">API Documentation</a>
<a class="text-xs font-bold text-primary hover:underline decoration-2 underline-offset-4" href="#">Security Policy</a>
<a class="text-xs font-bold text-primary hover:underline decoration-2 underline-offset-4" href="#">Support Hub</a>
</div>
</footer>
</div>
</main>
<!-- Contextual FAB (Only for main analysis screen) -->
<button class="fixed bottom-10 right-10 signature-gradient text-white w-14 h-14 rounded-full flex items-center justify-center ambient-shadow hover:scale-105 transition-transform duration-200 group">
<span class="material-symbols-outlined text-2xl" style="font-variation-settings: 'FILL' 1;">add</span>
<span class="absolute right-16 bg-primary-container text-on-primary-container px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap opacity-0 group-hover:opacity-100 transition-opacity">Compare New Version</span>
</button>
</body></html>