<?php
// ==========================================
//            PORTFOLIO CONFIGURATION - YOURS
// ==========================================

// 1. BASIC INFO
$name         = "KingTim17287";       
$roblox_id    = "3808496324";         
$for_hire     = "No";                 
$title        = "Roblox Developer";   
$title_color  = "blue-500";           
$bio          = ""; // not used anymore
$bio_color    = "white";              

// 2. THEME SETTINGS
$theme_color  = "blue";                
$accent_hex   = "#3b82f6";             
$avatar_animation = "Yes"; 

// 3. ADVANCED COLORS (HEX Codes)
$bg_color     = "#0b1120";             
$text_color   = "#f8fafc";             
$glass_bg     = "rgba(30, 41, 59, 0.5)"; 
$card_border  = "rgba(255, 255, 255, 0.08)"; 

// 4. SEO & META SETTINGS
$seo_title       = "KingTim17287 | Roblox Game Developer";
$seo_description = "My Roblox games: Jetpack over LAVA, Dead Meals, 99 Nights Zombie Tower Defense and more!";
$seo_keywords    = "Roblox, Developer, Portfolio";
$seo_image       = "";
$seo_favicon     = "";

// 7. YOUR 8 GAMES ONLY (placeIds from the links you gave)
$manualGameIds = [106988495261000, 77942507005261, 95744979554149, 104877476991790, 14044594226, 82126039807655, 101246660655753, 108311894104237];

// 8. YOUR 3 COMMUNITIES
$communities = [
    [
        "name" => "Boden Interactive",
        "desc" => "Official Group - Join for updates & events!",
        "id"   => "426353491",
        "link" => "https://www.roblox.com/communities/426353491/Boden-Interactive#!/about"
    ],
    [
        "name" => "Woven Productions",
        "desc" => "Official Group - Join for updates & events!",
        "id"   => "7457551",
        "link" => "https://www.roblox.com/communities/7457551/Woven-Productions#!/about"
    ],
    [
        "name" => "StarWoven Productions",
        "desc" => "Official Group - Join for updates & events!",
        "id"   => "35252165",
        "link" => "https://www.roblox.com/communities/35252165/StarWoven-Productions#!/about"
    ]
];

// ==========================================
//             CORE LOGIC (same as template)
// ==========================================
function fetchPortfolioData($userId) {
    $url = "https://api.un6107617.dev/portfolio/" . $userId;
    $ch = curl_init();
    curl_setopt($ch, CURLOPT_URL, $url);
    curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
    curl_setopt($ch, CURLOPT_FOLLOWLOCATION, true);
    curl_setopt($ch, CURLOPT_TIMEOUT, 5);
    curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, false);
    $result = curl_exec($ch);
    curl_close($ch);
    return json_decode($result, true);
}

$api_data = fetchPortfolioData($roblox_id);
$avatar_url = $api_data['user']['avatar'] ?? "";
$my_games = $api_data['games'] ?? [];

// Filter to ONLY your 8 games
$filtered_games = array_filter($my_games, function($game) use ($manualGameIds) {
    return in_array((int)$game['placeId'], $manualGameIds);
});
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title><?php echo $seo_title; ?></title>
    <meta name="description" content="<?php echo $seo_description; ?>">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root { --accent: <?php echo $accent_hex; ?>; }
        body { background-color: <?php echo $bg_color; ?>; color: <?php echo $text_color; ?>; scroll-behavior: smooth; }
        .glass { background: <?php echo $glass_bg; ?>; backdrop-filter: blur(12px); border: 1px solid <?php echo $card_border; ?>; }
        .img-container { aspect-ratio: 16/9; overflow: hidden; background: #111; }
        .img-container img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.5s ease; }
        .group:hover .img-container img { transform: scale(1.05); }
        .stat-card { background: rgba(255,255,255,0.05); border: 1px solid rgba(255,255,255,0.1); }
        .avatar-float { animation: float 4s ease-in-out infinite; }
        @keyframes float { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }
    </style>
</head>
<body class="antialiased tracking-tight">

<nav class="fixed top-0 w-full z-50 py-5 px-6 glass">
    <div class="max-w-6xl mx-auto flex justify-between items-center">
        <span class="font-black text-3xl italic uppercase tracking-tighter" style="color:var(--accent)"><?php echo $name; ?></span>
    </div>
</nav>

<div class="pt-32 pb-20 px-6 max-w-6xl mx-auto">

    <!-- AVATAR (same as template) -->
    <div class="text-center mb-12">
        <img src="<?php echo $avatar_url; ?>" class="w-64 h-64 mx-auto rounded-full border-8 shadow-2xl avatar-float" style="border-color:var(--accent)" alt="">
    </div>

    <!-- TOP TOTAL STATS -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-16">
        <div class="stat-card rounded-3xl p-8 text-center">
            <div class="text-6xl font-black italic text-emerald-400"><?php echo array_sum(array_column($filtered_games, 'playing')); ?></div>
            <p class="uppercase text-sm tracking-widest text-emerald-400/80 mt-2">PLAYERS PLAYING MY GAMES</p>
        </div>
        <div class="stat-card rounded-3xl p-8 text-center">
            <div class="text-6xl font-black italic text-blue-400"><?php echo array_sum(array_column($filtered_games, 'visits')); ?></div>
            <p class="uppercase text-sm tracking-widest text-blue-400/80 mt-2">TOTAL VISITS</p>
        </div>
    </div>

    <!-- MY GAMES (first) -->
    <section class="mb-16">
        <div class="flex items-center gap-3 mb-8">
            <div class="h-8 w-2" style="background:var(--accent)"></div>
            <h2 class="text-4xl font-black italic uppercase tracking-tighter">MY GAMES</h2>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <?php foreach($filtered_games as $game): ?>
            <div class="glass rounded-3xl overflow-hidden flex flex-col group">
                <div class="img-container"><img src="<?php echo $game['thumbnail']; ?>" alt=""></div>
                <div class="p-8">
                    <h3 class="text-2xl font-black mb-2"><?php echo $game['name']; ?></h3>
                    <p class="opacity-70 mb-6"><?php echo $game['description'] ?? 'No description'; ?></p>
                    <div class="flex justify-between text-xs mb-6">
                        <div>CCU <span class="font-black text-emerald-400"><?php echo number_format($game['playing'] ?? 0); ?></span></div>
                        <div>Visits <span class="font-black text-blue-400"><?php echo number_format($game['visits'] ?? 0); ?></span></div>
                    </div>
                    <a href="https://www.roblox.com/games/<?php echo $game['placeId']; ?>" target="_blank" class="font-black text-xs uppercase block text-center" style="color:var(--accent)">PLAY →</a>
                </div>
            </div>
            <?php endforeach; ?>
        </div>
    </section>

    <!-- MY COMMUNITIES -->
    <section>
        <div class="flex items-center gap-3 mb-8">
            <div class="h-8 w-2" style="background:var(--accent)"></div>
            <h2 class="text-4xl font-black italic uppercase tracking-tighter">MY COMMUNITIES</h2>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <?php foreach($communities as $g): ?>
            <div class="glass rounded-3xl overflow-hidden flex flex-col group">
                <div class="img-container">
                    <img src="https://thumbnails.roproxy.com/v1/groups/icons?groupIds=<?php echo $g['id']; ?>&size=420x420&format=Png" alt="">
                </div>
                <div class="p-8">
                    <h3 class="text-2xl font-black mb-2"><?php echo $g['name']; ?></h3>
                    <p class="opacity-70 mb-6"><?php echo $g['desc']; ?></p>
                    <a href="<?php echo $g['link']; ?>" target="_blank" class="font-black text-xs uppercase block text-center" style="color:var(--accent)">JOIN GROUP →</a>
                </div>
            </div>
            <?php endforeach; ?>
        </div>
    </section>

</div>

<footer class="glass py-8 text-center text-xs font-bold">© 2026 KingTim17287 • Template by UN6107617</footer>

</body>
</html>
