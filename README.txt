CHHAYA MEHNDI & ARTS - WEBSITE
==============================

Kaise chalayein
---------------
index.html par double-click karo, website browser me khul jayegi.
Hosting ke liye poora folder (index.html, style.css, script.js, images/) 
Netlify / Vercel / GitHub Pages / kisi bhi hosting par upload kar do.

Folder structure
----------------
index.html     -> page ka content (text, sections)
style.css      -> design, colours, responsive layout
script.js      -> gallery, filters, full-screen preview, WhatsApp links
images/        -> saari images (abhi sample images hain)
tools/         -> sample images banane ki script (zaroori nahi)

1) Apni images lagana (sabse zaroori)
-------------------------------------
images/ folder me ye 20 files hain. Apni photo ko SAME NAAM se save karke
purani file replace kar do, website apne aap nayi image dikha degi:

  mehndi-01.jpg ... mehndi-10.jpg   (10 Mehndi)
  art-01.jpg    ... art-10.jpg      (10 Painting / Art)
  chhaya.jpg                        (About section me Chhaya ki photo)

Tips:
- Extension .jpg hi rakho (ya script.js me file ka naam badal do).
- Width 1000-1400px kaafi hai, file 300KB se chhoti rakho (site fast chalegi).
- Portrait, landscape ya square - kisi bhi size ki photo chalegi,
  masonry gallery apne aap adjust kar leti hai.
- Replace ke baad purani image dikhe to browser cache ki wajah se hai:
  Ctrl + F5 (mobile par tab band karke dobara kholo).

2) WhatsApp number aur email badalna
------------------------------------
script.js ko kholo, sabse upar CONFIG me:

  whatsapp: '919999999999'   -> country code ke saath number (bina + aur space)
  phoneDisplay: '+91 99999 99999'
  email: 'hello@example.com'

Ek jagah badalne se poori website ke saare buttons update ho jate hain.

3) Image ke titles badalna
--------------------------
script.js me GALLERY list hai. Har line me title badal do, jaise:
  { file: 'mehndi-01.jpg', cat: 'mehndi', title: 'Bridal Vine Mehndi', feat: 1, shape: 'arch' }

  feat: 1/2/3  -> Featured Mehndi / Featured Art section me dikhegi
  shape: 'arch' -> upar se gol (mehrab) shape, sirf lambi (portrait) photo par lagao

4) Text badalna
---------------
About, Services, hero ka text index.html me hai. Jo text abhi likha hai wo
sample hai - apni asli kahani aur services se badal do.

5) Colours
----------
style.css ke shuru me :root me saare colours hain (cream, green, brown, gold).
