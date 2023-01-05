<script>
    const boardgamesList = [
            {
                title: 'Jenga',
                description: ['To klasyczna gra Jenga z oryginalnymi drewnianymi klockami! Gra Jenga to oryginalna gra z użyciem drewnianych klocków, którą rodziny kochają od pokoleń.'],
                img: '/library/jenga.jpg',
                link: 'https://boardgamegeek.com/boardgame/2452/jenga'
            },
            {
                title: 'Mistakos level',
                description: ['Mistakos to klasyczna gra zręcznościowa dla dzieci – i nie tylko! Walka o stołki z pewnością pochłonie również starszych graczy. Zapewnij swojej rodzinie wciągająca rozrywkę z nutką zdrowej rywalizacji!'],
                img: '/library/mistakos.png',
                link: 'https://boardgamegeek.com/boardgame/292908/mistakos-level'
            },
            {
                title: 'UNO Flip!',
                description: [
                    'Już od ponad 40 lat UNO bawi i cieszy graczy na całym świecie. To ta sama kultowa gra karciana, ale teraz z nowymi, ekscytującymi elementami – takimi jak dwustronne karty, specjalna karta ODWRÓĆ i ostrzejsze reguły – które podniosą poziom rywalizacji w rozgrywce.',
                ],
                img: '/library/uno-flip.jpg',
                link: 'https://boardgamegeek.com/boardgame/271460/uno-flip'
            },
                        {
                title: 'Światowy konflikt',
                description: [
                    'Walka o wpływy, pieniądze i władzę! Akcja gry toczy się w jednym z państw leżącychna granicy dwóch stref wpływów: rosyjskiej i zachodniej.',
                    'Gracze wcielają się w rolęlokalnych polityków starającymi się sięgnąć po władzę. Aby im się to udało, będą musieli skutecznie wykorzystać swoje wpływy w kraju i za granicą.'
                ],
                img: '/library/world_conflikt.jpg',
                link: 'https://allegro.pl/oferta/swiatowy-konflikt-imprezowa-gra-planszowa-coup-pl-11097193315'
            },
            {
                title: '6 nimmt',
                description: [
                    'Celem gry jest zebranie jak najmniejszej ilości kart. Każda karta jest warta minus jeden punkt za każdą głowę byka znajdującą się na niej. Zwycięzcą zostaje osoba, która na końcu gry ma najmniejszą ilość byczych głów.  ',
                    'Proste zasady, ale daje całkiem sporo pokerowych emocji.'
                ],
                img: '/library/6-bierze.jpg',
                link: 'https://boardgamegeek.com/boardgame/432/6-nimmt'
            },
            {
                title: 'Carcassonne',
                description: [
                    'Usiądź z przyjaciółmi przy stole i wspólnie zacznijcie budować z niewielkich żetonów łąki, twierdze, całe miasta i drogi, rywalizując między sobą o przejęcie kontroli nad co bardziej atrakcyjnymi lokacjami.',
                    'Sprytne zagranie może pozbawić rywala możliwości ukończenia ogromnego miasta lub pozwoli Ci przejąć kontrolę nad wielką łąką.'
                ],
                img: '/library/carcassonne.jpg',
                link: 'https://boardgamegeek.com/boardgame/822/carcassonne'
            },

            {
                title: 'K2',
                description: [
                    'K2 to rodzinna gra planszowa, w której uczestnicy kierują dwuosobowymi zespołami himalaistów i próbują zdobyć tytułowy szczyt, a następnie bezpiecznie zejść na dół. W tym celu będziemy musieli wybrać odpowiednią drogę, zadbać o kondycję naszych wspinaczy oraz ich zaadaptowanie do zmiennych warunków pogodowych.',
                    ''
                ],
                img: '/library/k2.jpg',
                link: 'https://boardgamegeek.com/boardgame/73761/k2'
            },
            {
                title: 'ATAK ZOMBIE',
                description: [
                    'Przygotuj się na atak zombie!',
                    'Nieznany wirus zaatakował ludzi przemieniając większość z nich w zombie. Nie ma czasu na robienie zapasów i długie przygotowania do ucieczki. Chcąc przeżyć, gracze muszą schronić się w jednej z podmiejskich lokacji i odpierać kolejne fale żywych trupów, aż do nadejścia pomocy. Muszą zapewnić sobie jedzenie, lekarstwa i broń. Aby je zdobyć zmuszeni są wychodzić z kryjówek narażając się na spotkanie zombie.'
                ],
                img: '/library/atak_zombie.jpg',
                link: 'https://boardgamegeek.com/boardgame/170344/atak-zombie'
            },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
            // {
            //     title: 'Lorem',
            //     description: [
            //         '',
            //         ''
            //     ],
            //     img: '/library/',
            //     link: ''
            // },
        ];
        
        

        
</script>

<div class="w-12/12 -mb-52 -mt-52 flex flex-row justify-center flex-wrap ">
<div style="background-color: #f3e600;" class="workshops-section rounded-2xl mb-12 mt-12 lg:w-7/12 px-8 sm:w-8/12 h-auto p-10 flex flex-col flex-wrap justify-center content-center ">
        <h2 class="lg:text-7xl text-5xl  text-center mb-2 text-dark font-impact">Wypożyczalnia gier planszowych</h2>

        <div class="flex flex-row w-full flex-wrap justify-center ">
        {#each boardgamesList as boardgame}
            <div class="m-1 bg-white dark:bg-gray-800 text-gray-500 dark:text-gray-400 rounded-lg border border-gray-200 dark:border-gray-700 shadow-md flex max-w-sm flex-col">
                <img style="" class="rounded-t-lg" src="{boardgame.img}" alt="{boardgame.title}"> 
                <div class="p-4 sm:p-6">
                    <h5 class="mb-2 text-2xl font-impact text-gray-700">
                        {boardgame.title}
                    </h5> 
                    {#each boardgame.description as text}
                        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
                            {text}
                        </p> 
                    {/each}
                       <a href='{boardgame.link}' class="w-full text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-white bg-dark hover:bg-dark focus:ring-blue-300 rounded-lg">
                            Czytaj więcej
                        </a>
                </div>
            </div>

        {/each}
    </div>
</div>
</div>
        

