<script>
  import CtAs from "./CTAs.svelte";
  import Header from "./Header.svelte";
  import SectionWrapper from "./SectionWrapper.svelte";
  import Stars from "./Stars.svelte";
</script>

<SectionWrapper>
  <Header />
  <div
    class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14"
  >
    <h2
      class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl max-w-[1200px] mx-auto w-full text-center font-semibold"
    >
      Treinamento na <span class="text-indigo-400">academia</span>
      <span class="text-slate-600 line-through">é difícil</span> <br />
      ficou <span class="text-indigo-400">mais fácil</span>
    </h2>
    <p
      class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] mx-auto w-full"
    >
      Pense menos e faça mais. Nós somos o seu treinador completo com
      <span class="italic">
        treinamento personalizado, explicações de exercícios, análises
      </span>
      e muito mais
    </p>
    <CtAs dark={false} />
    <Stars />
  </div>
</SectionWrapper>
