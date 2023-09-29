<script>
    import certificatesData from "../../certificates.json";

    let certifications = certificatesData;
</script>


<head>
    <title>Certifications - Prathamesh Dhawanjewar</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap" rel="stylesheet">
</head>
<body>
    <div class="all-cerf-container">
        {#each certifications as { title, links }, i}
            <div class="course">
                <h1>{title}</h1>
                <div class="cerf-images">
                    {#each links as { targetLink, source }, j}
                        <a href={targetLink} target="_blank">
                            <img src={source} alt="{i}.{j}" loading="lazy" />
                        </a>
                    {/each}
                </div>
            </div>
        {/each}
    </div>
</body>


<style>
    body{
        margin: 0;
        background-color: black;
    }
    .cerf-images {
        display: flex;
        height: 40%;
        overflow-x: scroll;
        padding: 10px;
        border-color: black;
    }
    .course h1 {
        text-align: center;
        color: white;
        padding-left: 10px;
        padding-right: 10px;
        font-size: 3vw;
        font-family: "Montserrat", sans-serif;
    }
    .cerf-images a img {
        width: 48vh;
        height: auto;
    }
</style>
