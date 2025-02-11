# Shop

🚀 Getting Started with React and Angular
Structura Aplicatiei mele web 
# 📦 Structura Proiectului - Aplicație Web Dropshipping

Aceasta este structura aplicației web pentru un magazin de dropshipping, construită folosind **React**. Aplicația este organizată pe componente modulare, pagini dedicate, hooks personalizate și servicii pentru gestionarea datelor.

## 🗂️ **Structura Generală a Proiectului**

/project-root
├── public/
├── src/
├── package.json
├── .gitignore
└── README.md

## 📁 **1. Folderul `public/`**

- **`index.html`** - Punctul de intrare al aplicației. Aici este montată aplicația React în DOM, folosind un div cu id-ul `root`.
- **`/images`** - Folder dedicat pentru stocarea imaginilor statice ale produselor. Aceste imagini sunt accesibile direct fără a fi procesate de Webpack.



## 📁 **2. Folderul `src/`**

Acesta conține toată logica aplicației React.

### 📄 **`index.js`**
- Fișierul principal de inițializare al aplicației.
- Aici se face legătura între `ReactDOM` și `index.html`.

### 📄 **`App.jsx`**
- Componenta principală care definește structura generală a aplicației.
- Include rutarea și layout-ul de bază.



## 📁 **3. Folderul `components/`**

Conține componente reutilizabile pentru diverse funcționalități:

- **`Header.jsx`** - Bara de navigare principală cu logo-ul și meniul de navigație.
- **`Footer.jsx`** - Footer-ul aplicației cu informații de contact, linkuri utile etc.
- **`ProductCard.jsx`** - Componentă pentru afișarea fiecărui produs individual (imagine, nume, preț, buton "Adaugă în coș").
- **`Pagination.jsx`** - Funcționalitate de paginare (8 produse pe pagină).
- **`ProductList.jsx`** - Listă de produse care suportă paginarea și filtrele.
- **`Cart.jsx`** - Gestionarea coșului de cumpărături (adăugare, eliminare, total).
- **`CheckoutForm.jsx`** - Formular pentru finalizarea comenzii (detalii de livrare, plată etc.).



## 📁 **4. Folderul `pages/`**

Conține paginile principale ale aplicației:

- **`Home.jsx`** - Pagina principală cu o prezentare generală a magazinului.
- **`Shop.jsx`** - Catalogul de produse cu funcționalitate de paginare.
- **`ProductPage.jsx`** - Pagina de detalii pentru un produs specific.
- **`CartPage.jsx`** - Pagina coșului de cumpărături cu posibilitatea de a modifica cantitățile sau de a elimina produse.
- **`Checkout.jsx`** - Pagina pentru finalizarea comenzii și trimiterea detaliilor către server.
- **`About.jsx`** - Pagina „Despre Noi”, cu informații despre companie.
- **`Contact.jsx`** - Pagina de contact cu formular de trimitere a mesajelor.


## 📁 **5. Folderul `hooks/`**

Conține hooks personalizate pentru logica aplicației:

- **`usePagination.js`** - Hook personalizat pentru logica de paginare, utilizat în `ProductList.jsx`.


## 📁 **6. Folderul `contexts/`**

Gestionarea stării globale a aplicației:

- **`CartContext.js`** - Context pentru gestionarea coșului de cumpărături. Permite accesarea și modificarea coșului din orice componentă.


## 📁 **7. Folderul `services/`**

Pentru gestionarea datelor și apelurilor API:

- **`productService.js`** - Serviciu pentru obținerea datelor despre produse. Poate conține apeluri către un API extern sau către un fișier JSON local.


## 📁 **8. Folderul `styles/`**

Pentru stiluri personalizate:

- **`main.css`** - Fișierul principal de stiluri. Poate conține reguli CSS personalizate, pe lângă cele generate de framework-uri precum Tailwind CSS.


## 📁 **9. Folderul `data/`**

Date statice pentru dezvoltare și testare:

- **`products.json`** - Fișier JSON cu date despre cele 40 de produse din catalog. Este folosit pentru a popula lista de produse în lipsa unui API real.

## 📦 **10. Fișiere de configurare**

- **`package.json`** - Conține configurările și dependențele proiectului (React, React Router, Tailwind CSS etc.).
- **`.gitignore`** - Listează fișierele și folderele care nu trebuie incluse în controlul versiunii (ex: `node_modules/`).
- **`README.md`** - Acest fișier. Oferă documentația de bază a proiectului.







