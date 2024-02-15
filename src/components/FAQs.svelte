<script>
    import SectionWrapper from "./SectionWrapper.svelte";
    let faqs = [
        {
            question: "O que é o Muscular Gym?",
            ans: "Muscular Gym é um divertido aplicativo de fitness projetado para tornar seus treinos agradáveis, incorporando jogos e desafios interativos.",
        },
        {
            question: "Como faço o download do Muscular Gym?",
            ans: "Você pode baixar Muscular Gym na App Store (para iOS) ou Google Play Store (para Android) em seu dispositivo móvel.",
        },
        {
            question: "O uso do Muscular Gym é gratuito?",
            ans: "Sim, o Muscular Gym oferece uma versão gratuita com recursos básicos. Há também uma assinatura premium que desbloqueia jogos adicionais e monitoramento avançado de exercícios.",
        },
        {
            question: "Que tipos de treino o Muscular Gym oferece?",
            ans: "Muscular Gym oferece uma variedade de exercícios, incluindo cardio, treinamento de força e exercícios de flexibilidade. Os treinos são projetados para serem envolventes e divertidos.",
        },
        {
            question: "Posso conectar o Muscular Gym ao meu monitor de fitness?",
            ans: "Sim, o Muscular Gym oferece suporte à integração com rastreadores de fitness populares, permitindo que você sincronize os dados do seu treino e acompanhe seu progresso perfeitamente.",
        },
        {
            question: "Existem recursos multijogador no Muscular Gym?",
            ans: "Sim, Muscular Gym inclui desafios multijogador, permitindo que você compita com amigos ou participe de treinos em grupo para uma experiência mais interativa e social.",
        },
        {
            question: "Como o Muscular Gym motiva os usuários a permanecerem ativos?",
            ans: "Muscular Gym emprega um sistema de recompensa, onde os usuários ganham pontos e conquistas ao completar os treinos. Essas recompensas podem ser usadas para desbloquear novos níveis, desafios e conteúdo no aplicativo.",
        },
        {
            question: "Posso personalizar meus treinos no Muscular Gym?",
            ans: "Absolutamente! Muscular Gym permite que os usuários personalizem seus treinos com base em preferências pessoais, metas de condicionamento físico e equipamentos disponíveis.",
        },
        {
            question: "Existe um modo amigável para iniciantes no Muscular Gym?",
            ans: "Sim, o Muscular Gym oferece um modo para iniciantes com exercícios mais fáceis e de menor intensidade, tornando-o adequado para usuários em vários níveis de condicionamento físico.",
        },
        {
            question:
                "Com que frequência devo usar Muscular Gym para obter melhores resultados?",
            ans: "A frequência dos treinos Muscular Gym depende de seus objetivos de condicionamento físico. Recomenda-se realizar pelo menos 3-5 sessões por semana para obter resultados visíveis.",
        },
    ];
</script>

<SectionWrapper id="faqs">
    <div
        class="flex flex-col gap-10 sm:gap-14 md:gap-24 py-20 flex-1 items-center justify-center"
    >
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                Para todas suas perguntas e dúvidas
            </p>
            <h3
                class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
            >
                Perguntas Frequentes
            </h3>
        </div>
        <div class="flex flex-col gap-8 sm:gap-10 md:gap-14 w-full">
            {#each faqs as faq}
                <div
                    class="flex flex-col gap-2 text-left max-w-[800px] w-full mx-auto relative p-4 px-6"
                >
                    <div
                        class="absolute top-0 left-0 w-1/3 h-[1px] bg-slate-950 -translate-x-4"
                    ></div>
                    <div
                        class="absolute top-0 left-0 h-2/3 w-[1px] bg-slate-950 -translate-y-4"
                    ></div>
                    <h4 class="text-lg sm:text-xl md:text-2xl pt-2">
                        {faq.question}
                    </h4>
                    <p class="pl-2">{faq.ans}</p>
                </div>
            {/each}
        </div>
    </div>
</SectionWrapper>