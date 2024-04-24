<script>
    import Footer from "$lib/footer.svelte";
</script>

<svelte:head>
  <meta name="theme-color" content="#FF5876"/>
  <meta name="description" content="Home of the Ksuite of tools">
  <title>Ksuite</title>
</svelte:head>

<main>
    <h1 class="center poppins">Welcome to</h1>
    <div class="logo-stack">
        <img
            class="center tool-logo bottom main-logo"
            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ksuite.svg"
            alt="Ksuite logo"
        />
        <img
            class="center top main-logo"
            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ksuite-no-blur.svg"
            alt="Ksuite logo"
        />
    </div>

    <h1 class="center poppins">Check out the tools below:</h1>
    <div class="center project-showcase">
        <div id="Ktool">
            <a class="tool-title" href="https://github.com/kociumba/ktool">
                <div class="showcase center ktool">
                    <h1 class="poppins">Ktool</h1>
                    <div class="logo-stack">
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ktool-ico.svg"
                            alt="Ktool"
                            class="tool-logo bottom font-offset"
                        />
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ktool-ico-no-blur.svg"
                            alt="Ktool"
                            class="top font-offset"
                        />
                    </div>
                </div>
            </a>
        </div>
        <div id="Ksorter">
            <a class="tool-title" href="https://github.com/kociumba/ksorter">
                <div class="showcase center ksorter">
                    <h1 class="poppins">Ksorter</h1>
                    <div class="logo-stack">
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ksorter-ico.svg"
                            alt="Ksorter"
                            class="tool-logo bottom font-offset"
                        />
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/ksorter-ico-no-blur.svg"
                            alt="Ksorter"
                            class="top font-offset"
                        />
                    </div>
                </div>
            </a>
        </div>
        <div id="Kinjector">
            <a class="tool-title" href="https://github.com/kociumba/Kinjector">
                <div class="showcase center kinjector">
                    <h1 class="poppins">Kinjector</h1>
                    <div class="logo-stack">
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/kinjector-ico.svg"
                            alt="Kinjector"
                            class="tool-logo bottom font-offset"
                        />
                        <img
                            src="https://raw.githubusercontent.com/kociumba/Ksuite/main/src/lib/kinjector-ico-no-blur.svg"
                            alt="Kinjector"
                            class="top font-offset"
                        />
                    </div>
                </div>
            </a>
        </div>
    </div>
    <Footer />
</main>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

    ::selection {
        background-color: #0000005e !important;
        color: #ffffff !important;
    }

    .center {
        text-align: center;
        display: block;
        margin-left: auto;
        margin-right: auto;
        color: white;
    }

    .project-showcase {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 10px;
        margin: 5vh;
    }

    .showcase {
        width: 20em; /* Scales based on the font size of its parent */
        height: 20em; /* Scales based on the font size of its parent */
        border-radius: 20px;
        padding: 5px;
    }

    .main-logo {
        width: 400px;
        height: 250px;
    }

    .tool-title {
        text-decoration: none;
    }

    .tool-logo {
        filter: blur(10px);
    }

    .logo-stack {
        display: grid;
    }

    .logo-stack img:nth-child(1) {
        margin-left: auto;
        margin-right: auto;
        grid-row: 1;
        grid-column: 1;
    }

    .logo-stack img:nth-child(2) {
        margin-left: auto;
        margin-right: auto;
        grid-row: 1;
        grid-column: 1;
    }

    .font-offset {
        margin-left: 50px !important;
    }

    .bottom {
        z-index: 1;
    }

    .top {
        z-index: 2;
    }

    .ktool {
        background: linear-gradient(135deg, #ffffff11 0%, #745777 100%);
        transition:
            transform 0.3s ease-in-out,
            box-shadow 0.3s ease-in-out;
        cursor: pointer;
    }

    .ktool:hover {
        transform: scale(1.05);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    .ksorter {
        background: linear-gradient(135deg, #ffffff11 0%, #a86d4a8a 100%);
        transition:
            transform 0.3s ease-in-out,
            box-shadow 0.3s ease-in-out;
        cursor: pointer;
    }

    .ksorter:hover {
        transform: scale(1.05);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    .kinjector {
        background: linear-gradient(135deg, #ffffff11 0%, #71c46e7c 100%);
        transition:
            transform 0.3s ease-in-out,
            box-shadow 0.3s ease-in-out;
        cursor: pointer;
    }

    .kinjector:hover {
        transform: scale(1.05);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    .poppins {
        font-family: "Poppins";
    }

    :global(html) {
        /* background: rgb(9, 9, 11); */
        background: linear-gradient(-160deg, #1d0f11 0%, #000000 100%);
        min-height: 100vh;
        margin: 0;
        overflow: visible;
    }
</style>
