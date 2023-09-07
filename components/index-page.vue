<template lang="pug">
div
    .title.my-10
        h1.text-4xl.font-bold.leading-normal.tracking-tight.m-0 KeumJeongSW 동아리 문서
        h2.text-xl.text-gray-600.mt-3 동아리, 무한 상상실 장비 관련 주의 사항이나 사용방법을 정리해놓은 문서입니다.
    hr
    .my-10.grid.grid-cols-1.gap-4(class="lg:grid-cols-2")
        .flex.flex-col.gap-5
            h2.font-bold.pt-5.text-3xl.mt-0.mb-0.tracking-tight 자주 찾는 질문
            h3.text-lg.mt-5.text-gray-500 자주 사용하는 기계들의 설명과 주의사항들을 모았습니다.
            p.my-3
                nuxt-link(to="/category/faq")
                    button.w-full.flex-none.bg-gray-900.text-white.leading-6.py-2.px-3.border.border-transparent.rounded-lg.transition.duration-200(class="sm:w-auto hover:bg-gray-700 focus:ring-offset-2 focus:ring-offset-white focus:ring-gray-900 focus:outline-none focus:ring-2")
                        | 탐색하기
                        i.fal.fa-arrow-right.ml-2
            .flex
                span.tag.bg-gray-200.p-2.text-sm.rounded-lg.text-gray-500 FAQ
                span.tag.bg-gray-200.p-2.text-sm.rounded-lg.text-gray-500 자주 찾는 질문
        img.w-full.h-auto.overflow-hidden.rounded-md.row-start-1(class="lg:row-start-auto" src="~/assets/img/index/faq_left.jpeg")

    hr
    .my-10.grid.grid-cols-1.gap-8(class="lg:grid-cols-3")
        .rounded-xl.bg-gradient-to-br.from-cyan-400.to-blue-500.p-5.text-white.flex.flex-col.gap-5
            h2.font-bold.text-2xl 컴퓨터실 가이드
            h3 컴퓨터실에서 사용하는 장비들의 설명과 주의사항을 확인해보세요!
            .flex-grow
            nuxt-link(to="/category/tutorials/computer")
                button.w-full.flex-none.bg-gray-900.bg-opacity-20.text-white.leading-6.py-2.px-3.border.border-transparent.rounded-lg.transition.duration-200(class="sm:w-auto hover:bg-gray-700 focus:ring-offset-2 focus:ring-offset-white focus:ring-gray-900 focus:outline-none focus:ring-2")
                    | 지금 확인하기
                    i.fal.fa-arrow-right.ml-2
        .rounded-xl.bg-gradient-to-br.from-yellow-400.to-orange-500.p-5.text-white.flex.flex-col.gap-5
            h2.font-bold.text-2xl 무한상상실 가이드
            h3 무한상상실에서 사용하는 장비들의 설명과 주의사항을 확인해보세요!
            .flex-grow
            nuxt-link(to="/category/tutorials/workplace")
                button.w-full.flex-none.bg-gray-900.bg-opacity-20.text-white.leading-6.py-2.px-3.border.border-transparent.rounded-lg.transition.duration-200(class="sm:w-auto hover:bg-gray-700 focus:ring-offset-2 focus:ring-offset-white focus:ring-gray-900 focus:outline-none focus:ring-2")
                    | 지금 확인하기
                    i.fal.fa-arrow-right.ml-2
        .rounded-xl.bg-gradient-to-br.from-green-400.to-green-600.p-5.text-white.flex.flex-col.gap-5
            h2.font-bold.text-2xl 기타 가이드
            h3 나머지 주의사항과 가이드들을 확인해보세요.
            .flex-grow
            nuxt-link(to="/category/tutorials/other")
                button.w-full.flex-none.bg-gray-900.bg-opacity-20.text-white.leading-6.py-2.px-3.border.border-transparent.rounded-lg.transition.duration-200(class="sm:w-auto hover:bg-gray-700 focus:ring-offset-2 focus:ring-offset-white focus:ring-gray-900 focus:outline-none focus:ring-2")
                    | 지금 확인하기
                    i.fal.fa-arrow-right.ml-2
    hr
    .my-10.grid.grid-cols-1.gap-4(class="lg:grid-cols-3")
        a.flex.items-center.text-sm(href="https://discord.gg/Kz77wGb6rw" target="_blank")
            .community-icon.rounded-lg.bg-gray-800.flex.items-center.justify-center.mr-3
                i.fab.fa-discord.text-white.text-lg
            .flex.flex-col
                h2.font-bold.text-2xl Discord(School)
                h3.text-gray-600 금정고등학교 학교 디스코드 서버로 이동합니다.
        a.flex.items-center.text-sm(href="https://discord.gg/M6aBeBXHKe" target="_blank")
            .community-icon.rounded-lg.bg-green-600.flex.items-center.justify-center.mr-3
                i.fab.fa-discord.text-white.text-lg
            .flex.flex-col
                h2.font-bold.text-2xl Discord(SW)
                h3.text-gray-600 금정고등학교 소프트웨어 동아리 디스코드 서버로 이동합니다.
        a.flex.items-center.text-sm(href="https://localhost:3000" target="_blank")
            .community-icon.rounded-lg.bg-black.flex.items-center.justify-center.mr-3
                i.fas.fa-terminal.text-white.text-lg
            .flex.flex-col
                h2.font-bold.text-2xl 준비중
                h3.text-gray-600 준비중인데용?
</template>

<script>
export default {
    name: "index-page"
}
</script>

<style lang="postcss">
.community-icon {
    width: 50px;
    height: 50px;
    max-width: 50px;
    max-height: 50px;
    min-width: 50px;
    min-height: 50px;
    padding: 10px;
}

.tag + .tag {
    margin-left: 6px;
}
</style>
