<script lang="ts">
    export const socials = [
        {
            icon: 'github',
            href: 'https://github.com/zhixuan2333',
            svg: '<path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" />'
        },
        {
            icon: 'twitter',
            href: 'https://twitter.com/zhixuan2333',
            svg: '<path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M22 4.01c-1 .49 -1.98 .689 -3 .99c-1.121 -1.265 -2.783 -1.335 -4.38 -.737s-2.643 2.06 -2.62 3.737v1c-3.245 .083 -6.135 -1.395 -8 -4c0 0 -4.182 7.433 4 11c-1.872 1.247 -3.739 2.088 -6 2c3.308 1.803 6.913 2.423 10.034 1.517c3.58 -1.04 6.522 -3.723 7.651 -7.742a13.84 13.84 0 0 0 .497 -3.753c-.002 -.249 1.51 -2.772 1.818 -4.013z" />'
        },
        {
            icon: 'mail',
            href: 'mailto:mailto:59254886+zhixuan2333@users.noreply.github.com',
            svg: '<path stroke="none" d="M0 0h24v24H0z" fill="none"/><rect x="3" y="5" width="18" height="14" rx="2" /><polyline points="3 7 12 13 21 7" />'
        },
        {
            icon: 'blog',
            href: 'https://blog.zhixuan.dev',
            svg: '<path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M6 4h11a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-11a1 1 0 0 1 -1 -1v-14a1 1 0 0 1 1 -1m3 0v18" /><line x1="13" y1="8" x2="15" y2="8" /><line x1="13" y1="12" x2="15" y2="12" />'
        }
    ];
    export const name = 'zhixuan';
    import '../app.css';
</script>

<svelte:head>
    <title>{name}</title>
    <meta name="description" content="student / Back-end / CN & JA & EN" />
    <meta name="robots" content="index,follow" />
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:site" content="@zhixuan2333" />
    <meta name="twitter:creator" content="@zhixuan2333" />
    <meta property="og:title" content={name} />
    <meta property="og:type" content="website" />
    <meta property="og:image" content="https://www.zhixuan.dev/og-image.png" />
    <meta property="og:image:alt" content={name} />
    <meta property="og:image:width" content="1920" />
    <meta property="og:image:height" content="1080" />
    <meta property="og:locale" content="en_US" />
    <meta property="og:site_name" content={name} />

    <script
        async
        src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12/lib/typed.min.js"
        integrity="sha256-UVQ5HtHTmtqBT3KY5cd4AvI47pp0gJwIM+q45HD9oLk="
        crossorigin="anonymous"></script>
</svelte:head>

<section class="bg-gray-100 min-h-screen flex items-center justify-center font-mono py-8">
    <div class="flex md:flex-row flex-col md:w-2/3 sm:w-3/5 w-4/5 items-center md:gap-16 gap-6">
        <div class="flex flex-col md:gap-6 gap-4 items-center">
            <div class="lg:w-56 w-40">
                <img
                    class="rounded-full"
                    alt="Avatar for {name}"
                    width="300"
                    height="300"
                    src="https://res.cloudinary.com/zhixuan/image/upload/c_scale,f_auto,h_300/v1642933312/avatar_ig7vzi.png"
                />
            </div>
            <div class="flex flex-col items-center gap-4">
                <h1 class="md:text-3xl text-2xl font-bold">{name}</h1>
                <div class="flex flex-row gap-4">
                    {#each socials as social}
                        <a href={social.href} class="social-item">
                            <svg
                                xmlns="http://www.w3.org/2000/svg"
                                viewBox="0 0 24 24"
                                width="24"
                                height="24"
                                stroke-width="1.5"
                                fill="none"
                                stroke-linecap="round"
                                stroke-linejoin="round"
                            >
                                {@html social.svg}
                            </svg>
                            <p>{social.icon}</p>
                        </a>
                    {/each}
                </div>
            </div>
        </div>
        <div class="flex flex-col gap-8">
            <div class="md:text-2xl text-xl">
                <p>Hi, I’m {name}. A <span class="typing text-orange-600" />.</p>
            </div>
            <div class="lg:text-lg text-base">
                <p>
                    Since I was a child, I like to make some things with my hands. Later, I learned
                    about Python and Golang, and now I am making some programs. Some of them are
                    open source. You can find them on GitHub. Currently, I am interested in
                    back-end. Recently, I started learning about front-end, so I made this
                    website✨. And I can speak Chinese, Japanese, and a little English.
                </p>
                <script>
                    window.onload = function () {
                        new Typed('.typing', {
                            strings: ['student', 'programmer'],
                            typeSpeed: 100,
                            backSpeed: 50,
                            backDelay: 1000,
                            loop: true
                        });
                    };
                </script>
            </div>
        </div>
    </div>
</section>

<!-- Please don't romove it!!! -->
<footer class="footer flex md:flex-row flex-col gap-2 text-xs md:text-sm">
    <p>
        Design By <a
            href="https://github.com/zhixuan2333/sinpuru"
            class="text-orange-600"
            target="_blank"
            rel="noopener"
            >zhixuan
        </a>.
    </p>
    <p>© 2020 - 2021 All right reserved.</p>
</footer>

<style lang="scss">
    .social-item {
        @apply flex flex-col items-center;
        svg {
            @apply w-6 stroke-gray-600;
        }
        p {
            @apply text-xs;
        }
    }
    .footer {
        @apply bg-gray-100 h-12 w-full items-center justify-center;
    }
</style>
