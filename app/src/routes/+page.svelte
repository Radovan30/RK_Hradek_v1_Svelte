<script context="module">
    import Nav from '../components/nav.svelte'
    import Hero from '../components/hero.svelte'
    import Card from '../components/card.svelte'
    import Gallery from '../components/gallery.svelte'
    import PreFooter from '../components/pre-footer.svelte'
    import Footer from '../components/footer.svelte'
</script>

<header>
    <Nav />
    <Hero />
</header>

<main>
    <Card/>
    <Gallery/>
</main>

<footer>
    <PreFooter />
    <Footer />
</footer>