<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SK Group of Education - GK & Science Portal</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- jsPDF & html2canvas for PDF Generation -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
    
    <style>
        /* Anti-Copy and Anti-Selection Protection */
        body {
            -webkit-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f5f9;
        }
        ::-webkit-scrollbar-thumb {
            background: #6366f1;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans min-h-screen flex flex-col justify-between">

    <!-- Header / Branding -->
    <header class="bg-indigo-700 text-white shadow-lg sticky top-0 z-40">
        <div class="max-w-7xl mx-auto px-4 py-4 flex flex-wrap justify-between items-center gap-4">
            <div class="flex items-center gap-3">
                <div class="bg-white text-indigo-700 p-2.5 rounded-xl font-black text-2xl shadow-md">
                    SK
                </div>
                <div>
                    <h1 class="text-xl sm:text-2xl font-bold tracking-tight">SK Group of Education</h1>
                    <p class="text-xs text-indigo-200">Interactive Science & GK Learning Platform (Class 1 - 9)</p>
                </div>
            </div>

            <!-- Action Controls -->
            <div class="flex items-center gap-2 sm:gap-3">
                <button onclick="openHostingModal()" class="bg-indigo-800 hover:bg-indigo-900 text-xs sm:text-sm px-3 py-2 rounded-lg transition flex items-center gap-1.5 border border-indigo-500/30">
                    <i class="fa-solid fa-globe text-indigo-300"></i>
                    <span>Get Public Link</span>
                </button>
                <div id="authContainer">
                    <button id="loginBtn" onclick="openLoginModal()" class="bg-amber-500 hover:bg-amber-600 text-slate-950 font-semibold text-xs sm:text-sm px-3.5 py-2 rounded-lg transition shadow-md flex items-center gap-1.5">
                        <i class="fa-solid fa-user-shield"></i>
                        <span>Founder Login</span>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content Container -->
    <main class="max-w-7xl mx-auto px-4 py-6 w-full flex-grow">
        
        <!-- Welcome Banner & Controls -->
        <div class="bg-white p-5 rounded-2xl shadow-sm border border-slate-200 mb-6 flex flex-col md:flex-row justify-between items-center gap-4">
            <div>
                <span id="editorStatusBadge" class="inline-block bg-indigo-50 text-indigo-700 text-xs font-semibold px-2.5 py-1 rounded-full mb-2 border border-indigo-200">
                    <i class="fa-solid fa-eye text-xs mr-1"></i> Public View-Only Mode
                </span>
                <h2 class="text-lg font-bold text-slate-900">Select Class to Explore GK & Science</h2>
                <p class="text-xs text
