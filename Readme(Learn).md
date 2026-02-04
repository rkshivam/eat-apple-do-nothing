// ISME MAI SARA THOUGHT PROCESS AND WHY LIKHUNGA SO THAT WHEN YOU WANT TO START ANY PROJECT YOU HAVE STARTING PART AND IDEA

@-> Use semantic tags (<main>, <section>, <header>, <footer>, <article>) whenever possible → better accessibility + SEO.

@-> <main> = the whole book (the main story of the page).
@-> <section> = the chapters inside the book (different topics within the main content).

@-> Example 
<main>
  <section>
    <h2>Introduction</h2>
    <p>Welcome to my blog...</p>
  </section>

  <section>
    <h2>Details</h2>
    <p>Here are the full details...</p>
  </section>
</main>

@-> Span (jab sentence mai sirf kisi word ke upar kam karna ho toh usko sapn mai daldo )
   <div> block-level hota hai (naya line le leta hai), par kabhi kabhi hume sirf ek chhoti wrapping chahiye hoti hai jo line ke andar hi rahe.

   Isi liye <span> bana: ek inline box jo semantic meaning nahi deta, bas grouping karta hai.
   <p>
      My favorite color is <span style="color: red;">red</span>.
   </p>
    Yahaan sirf "red" word ko style kiya gaya hai, pura paragraph nahi.

@-> What is Variable inside CSS root ?
    
    This Makes our website consistent design wise acrros all pages.
    root ke andar defined variables inherit hote hain → har child element unhe access kar sakta hai.
    Agar tum variables kisi aur selector mein define karte ho (jaise .container), toh wo sirf us container ke andar hi available hote hain.
    Isliye :root ek global scope banata hai.

@-> Example of using CSS variable
:root {
  --primary-color: blue;
  --font-size: 16px;
}

h1 {
  color: var(--primary-color);
  font-size: var(--font-size);
}

@-> IMP POINT
   🌱 Need (kyun -- lagana padta hai)
   CSS variables ko custom properties kehte hain.
   Browser ko ye batane ke liye ki "ye ek variable hai, normal property nahi," ek special prefix chahiye hota hai.
   Isliye -- prefix mandatory hai → bina iske browser usse variable nahi samjhega.

@-> what is html{}
    Matlab: jo bhi style tum html {} ke andar likhoge, wo poore page par apply hoga (kyunki har element <html> ke andar hi hota hai).


