# SewaBot
SEWAAN BOT PANCING MUARA GAYANG
<!DOCTYPE html>
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>XKUMPAU ANGLERS FISHING GROUP</title>
    <style>
        :root { --primary: #003049; --accent: #f77f00; --green: #25D366; --blue: #0077b6; }
        body { font-family: 'Poppins', sans-serif; margin: 0; background: #fdf0d5; color: #333; line-height: 1.6; }
        header { 
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('https://images.unsplash.com/photo-1544551763-46a013bb70d5?auto=format&fit=crop&w=1200&q=80');
            background-size: cover; background-position: center;
            color: white; padding: 60px 20px; text-align: center;
        }
        .container { max-width: 900px; margin: -30px auto 40px; background: white; padding: 25px; border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
        .grid-bot { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; margin-bottom: 25px; }
        .bot-card { border: 2px solid #eee; border-radius: 15px; padding: 15px; text-align: center; background: #f9f9f9; }
        .price { font-size: 22px; font-weight: bold; color: var(--accent); display: block; }
        .suitability { font-size: 13px; color: #666; font-style: italic; margin-bottom: 10px; }
        
        .section-title { border-left: 5px solid var(--accent); padding-left: 10px; margin: 20px 0 10px; color: var(--primary); }
        form { display: grid; gap: 15px; }
        label { font-weight: bold; font-size: 14px; }
        input, select, textarea { padding: 12px; border: 2px solid #ddd; border-radius: 10px; font-size: 16px; width: 100%; box-sizing: border-box; }
        
        /* Style untuk Pilihan Umpan */
        .umpan-selection { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; background: #f1f3f5; padding: 15px; border-radius: 10px; }
        .umpan-item { display: flex; align-items: center; gap: 8px; font-size: 14px; }
        .umpan-item input { width: auto; }

        .btn-submit { background: var(--accent); color: white; border: none; padding: 18px; border-radius: 10px; font-size: 18px; font-weight: bold; cursor: pointer; }
        .wa-container { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 15px; }
        .whatsapp-btn { color: white; text-decoration: none; display: block; text-align: center; padding: 12px; border-radius: 10px; font-weight: bold; font-size: 13px; }
        .maps-btn { background: var(--blue); color: white; text-decoration: none; display: block; text-align: center; padding: 12px; border-radius: 10px; margin-bottom: 20px; font-weight: bold; }
        @media (max-width: 600px) { .wa-container { grid-template-columns: 1fr; } .umpan-selection { grid-template-columns: 1fr; } }
    </style>
</head>
<body>

<header>
    <h1>⚓ XKUMPAU ANGLERS FISHING GROUP</h1>
    <p>Tuaran | Target: Siakap, MJ & GT</p>
</header>

<div class="container">
    <a href="https://maps.google.com/?q=5.163074,116.142514" target="_blank" class="maps-btn">📍 LOKASI JETI MUARA GAYANG</a>

    <h3 class="section-title">Katalog Bot & Harga</h3>
    <div class="grid-bot">
        <div class="bot-card">
            <h3>Bot 12 Kaki (5HP)</h3>
            <span class="price">RM100</span>
            <p class="suitability">Sesuai untuk: Casting Solo / 2 orang</p>
        </div>
        <div class="bot-card">
            <h3>Bot 16 Kaki (9.8HP)</h3>
            <span class="price">RM130</span>
            <p class="suitability">Sesuai untuk: 3-4 orang (Stabil)</p>
        </div>
        <div class="bot-card">
            <h3>Bot 21 Kaki (15HP)</h3>
            <span class="price">RM160</span>
            <p class="suitability">Sesuai untuk: Trip Family / 5-6 orang</p>
        </div>
    </div>

    <form action="https://formspree.io/f/xdayqpde" method="POST">
        <h3 class="section-title">Borang Tempahan</h3>
        
        <input type="text" name="Nama" placeholder="Nama Penuh" required>
        <input type="tel" name="WhatsApp" placeholder="No. WhatsApp" required>
        <input type="date" name="Tarikh" required>

        <label>Pilih Bot:</label>
        <select name="Pilihan_Bot" required>
            <option value="Bot_12ft">Bot 12 Kaki (RM100)</option>
            <option value="Bot_16ft">Bot 16 Kaki (RM130)</option>
            <option value="Bot_21ft">Bot 21 Kaki (RM160)</option>
        </select>

        <label>Tambah Tekong?</label>
        <select name="Tekong">
            <option value="Tidak">Tidak (Sewa Bot Sahaja)</option>
            <option value="Ya">Ya (Tambah RM50)</option>
        </select>

        <label>Pilihan Umpan (Boleh pilih banyak):</label>
        <div class="umpan-selection">
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Udang_30sen"> Udang (30¢)</div>
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Udang_50sen"> Udang (50¢)</div>
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Udang_80sen"> Udang (80¢)</div>
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Udang_RM1"> Udang (RM1)</div>
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Belanak"> Belanak (RM2)</div>
            <div class="umpan-item"><input type="checkbox" name="Umpan[]" value="Umpan_Mati"> Umpan Mati (RM5)</div>
        </div>

        <textarea name="Nota" rows="2" placeholder="Nyatakan kuantiti umpan (Cth: Udang 50 ekor)"></textarea>

        <button type="submit" class="btn-submit">H
