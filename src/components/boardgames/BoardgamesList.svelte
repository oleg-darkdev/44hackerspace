<script>
    import BoardgamesCategory from "./BoardgamesCategory.svelte";

    const cooperativeGames = [
        {
            name: 'Lorem ',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. ',
            images: [
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3toEO9Jfxu9f499DnfEg2wHaE1%26pid%3DApi&f=1&ipt=ceb1599f0081b7f5020760588479c02963da69e5d19341e0b3162b11fb4236f8&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.Glspgv49Iu--8ZgFermRpQHaE5%26pid%3DApi&f=1&ipt=58cd472fb2b3452ff300f53bcab1aed0bed3284ba1de9baba4d7d339e7a05ac6&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3sD54Xi4QoIKXwD3iPNUIgHaDt%26pid%3DApi&f=1&ipt=c9230a55e37f8d9d6ffafc76a8af960b597e48d124f6103b380c1827878d2806&ipo=images',
            ],
            link: ''
        },
        {
            name: 'Lorem ',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. ',
            images: [
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3toEO9Jfxu9f499DnfEg2wHaE1%26pid%3DApi&f=1&ipt=ceb1599f0081b7f5020760588479c02963da69e5d19341e0b3162b11fb4236f8&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.Glspgv49Iu--8ZgFermRpQHaE5%26pid%3DApi&f=1&ipt=58cd472fb2b3452ff300f53bcab1aed0bed3284ba1de9baba4d7d339e7a05ac6&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3sD54Xi4QoIKXwD3iPNUIgHaDt%26pid%3DApi&f=1&ipt=c9230a55e37f8d9d6ffafc76a8af960b597e48d124f6103b380c1827878d2806&ipo=images',
            ],
            link: ''
        },
        {
            name: 'Lorem ',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. ',
            images: [
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3toEO9Jfxu9f499DnfEg2wHaE1%26pid%3DApi&f=1&ipt=ceb1599f0081b7f5020760588479c02963da69e5d19341e0b3162b11fb4236f8&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.Glspgv49Iu--8ZgFermRpQHaE5%26pid%3DApi&f=1&ipt=58cd472fb2b3452ff300f53bcab1aed0bed3284ba1de9baba4d7d339e7a05ac6&ipo=images',
                'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.3sD54Xi4QoIKXwD3iPNUIgHaDt%26pid%3DApi&f=1&ipt=c9230a55e37f8d9d6ffafc76a8af960b597e48d124f6103b380c1827878d2806&ipo=images',
            ],
            link: ''
        },
    ]
</script>

<BoardgamesCategory gamesList={cooperativeGames}/>
