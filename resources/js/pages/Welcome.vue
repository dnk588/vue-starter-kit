<script setup lang="ts">
import { Head, Link } from '@inertiajs/vue3';
</script>

<template>
    <Head title="Юридическая фирма Ай Пи Про">
        <link rel="preconnect" href="https://rsms.me/" />
        <link rel="stylesheet" href="https://rsms.me/inter/inter.css" />
    </Head>
    <div class="relative min-h-screen flex items-center justify-center bg-gradient-to-br from-[#e0e7ef] via-[#f8fafc] to-[#c7d2fe] dark:from-[#18181b] dark:via-[#23232b] dark:to-[#1e293b] overflow-hidden">
        <!-- Эффект размытого фона -->
        <div class="absolute inset-0 z-0 bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-[#f53003]/10 via-[#c7d2fe]/30 to-transparent blur-2xl"></div>
        <div class="relative z-10 w-full max-w-lg p-1 rounded-3xl bg-gradient-to-br from-[#f53003] via-[#c7d2fe] to-[#e0e7ef] shadow-2xl">
            <div class="bg-white/80 dark:bg-[#18181b]/80 rounded-[22px] p-10 flex flex-col items-center backdrop-blur-xl border border-white/40 dark:border-[#edecec]/20">
                <img src="/images/logo.jpg" alt="Логотип Ай Пи Про" class="w-28 h-28 mb-6 rounded-full shadow-xl border-4 border-[#f53003]/60 bg-white object-contain transition-transform duration-300 hover:scale-105" />
                <h1 class="text-3xl font-extrabold text-[#1b1b18] dark:text-[#edecec] mb-2 text-center drop-shadow-lg tracking-tight">Юридическая фирма <br /> «Ай Пи Про»</h1>
                <div class="text-[#f53003] dark:text-[#FF4433] font-semibold text-lg mb-4 text-center animate-fade-in">Патентование и защита интеллектуальной собственности</div>
                <p class="text-base text-[#374151] dark:text-[#a1a09a] mb-8 text-center leading-relaxed max-w-md">
                    Юридическая фирма «Ай Пи Про» предлагает помощь при патентовании объектов интеллектуальной собственности в России и за рубежом. Мы гарантируем наилучшее качество и высокую скорость выполнения всех работ.
                </p>
                <div class="flex flex-col gap-4 w-full mt-2">
                    <Link
                        :href="route('login')"
                        class="w-full inline-block rounded-xl bg-gradient-to-r from-[#f53003] to-[#c7d2fe] text-white py-3 font-bold text-lg shadow-lg hover:from-[#c7d2fe] hover:to-[#f53003] hover:scale-105 transition-all duration-200 focus:outline-none focus:ring-2 focus:ring-[#f53003]/60"
                    >
                        &nbsp;&nbsp;&nbsp;Войти
                    </Link>
                    <Link
                        :href="route('register')"
                        class="w-full inline-block rounded-xl border-2 border-[#f53003] bg-white/70 text-[#f53003] py-3 font-bold text-lg shadow-lg hover:bg-[#f53003] hover:text-white hover:scale-105 transition-all duration-200 focus:outline-none focus:ring-2 focus:ring-[#f53003]/60 dark:bg-[#18181b]/70 dark:text-[#FF4433] dark:border-[#FF4433] dark:hover:bg-[#FF4433] dark:hover:text-white"
                    >
                    &nbsp;&nbsp;&nbsp;Регистрация
                    </Link>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@keyframes fade-in {
  from { opacity: 0; transform: translateY(-10px); }
  to { opacity: 1; transform: translateY(0); }
}
.animate-fade-in {
  animation: fade-in 1.2s cubic-bezier(.4,0,.2,1) both;
}
</style>
