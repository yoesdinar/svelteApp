# Svelte Demo App
ini adalah demo app menggunakan svelte. 
- clone repo ini 
- npm i
- npm run dev
- buka localhost:5000

nodejs required ya.

# Pengenalan
Bagaimana jika saya katakan svelte bukanlah sebuah framework? ternyata dia sebuah compiler. 🤯 

Mengutip dari website resmi svelte:
_Svelte is a radical new approach to building user interfaces. Whereas traditional frameworks like React and Vue do the bulk of their work in the browser, Svelte shifts that work into a compile step that happens when you build your app.
Instead of using techniques like virtual DOM diffing, Svelte writes code that surgically updates the DOM when the state of your app changes._

# Why Svelte
Untuk mengenal svelte, dan juga background dari pengembangannya, sangat disarankan untuk melihat video dari pengembangnya Rich Harris.

_Rich Harris - Rethinking Reactivity_

https://www.youtube.com/watch?v=AdNJ3fydeao

Beberapa catatan di video tersebut:
1. New framework is compiler
2. We need to rethink on how reactive should be
  1. on react, vue and other framework they use virtual DOM
  2. virtual DOM is an overhead, it is slow.
  3. is react slow? yes, how? the framework speak itself, they exposed shouldComponentUpdate, pure component etc.
3. Svelte already goes to version 3, 
  1. it already move reactivity out of the component API and into the language
4. SSR? instead of create component tree and serializing it, svelte concanitate strings and it should work faster.
  1. AWS bills will be lower
5. React code for same app is 40% more than similar app in svelte

# Another Svelte Benefit

1. Accessibility
2. Scoped Styles
    1. jadi gausah pake classes lagi, soalnya udah scoped dalem komponen
    2. bahkan child component ga bakal terpengaruh
    3. dia bikin hash buat class nya.
    4. ada CSS warning, kapan dia ga dipake atau dipake si kelas css nya
3. Transitions!
    1. bagus buat notif dll
    2. cuman tambah transition:fly{{y:250}} direction
    3. ada juga fade.
    4. spin function, css method
    5. ada parameter in and out
4. Complex Transitions
    1. move gracefully 
    2. transition using CSS -> not main thread jadi performa nya tinggi
5. Svelte is compiler
    1. not framework, ga bakal dateng file size gede si js nya.

# Svelte comparison with other
in a nutshell

![alt text](https://miro.medium.com/max/552/1*xxUbJTpBQmRPssfBZAjiqg.png)

![alt text](https://miro.medium.com/max/552/1*i8BONotbEvETZ4l_0rRigQ.png)

Svelte Another benefit (according to its founder)

# What experience did you get when developing with svelte?

Banyak yang rekomen pakai svelte, karena mereka ngerasa lebih seperti ngoding HTML daripada ngoding suatu framework.
kemudahan-kemudahan yang biasa kita dapatkan dari framework juga didapat disini. apalagi untuk reactivity, sangat intuitif.
tidak perlu lagi pakai define-define set dan setstate seperti di react untuk mengupdate variable.

Tidak perlu juga setting-setting webpack karena bundle size dari Svelte App sudah kecil.
fyi: bundlesize untuk project (bundle.js) ini adalah 21kb. cukup kecil dibanding yang lain.

# Beyond Svelte
Beyond Svelte
1. Sapper!
    1. Gatsby-style framework
    2. less js
    3. SSR and code splitting
2. Svelte native
    1. basedon nativescript-vue
3. Svelte GL
    1. like Three.js, but svelter
    
# Projects that suitable using Svelte
Seperti yang dijelaskan sebelumnya, tahun 2019 Svelte sudah masuk versi 3.
dari sisi popularitas, Svelte sekarang sedang mulai menanjak. namun dibanding bahasa js yang lain, Svelte masih kurang dalam hal komunitas.

Akan tetapi, untuk membuat sebuah aplikasi dengan tujuan utama performa, ringan, kode nya sedikit, dan tidak membutuhkan fitur-fitur library yang besar, Svelte.js patut untuk dilirik dan dicoba digunakan.


cheers. 
