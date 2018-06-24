<template>
    <div class="container">
        <div class="content">
            <Article v-for="(article, index) in articles" :article="article" :index="index"></Article>
        </div>
    </div>
</template>

<script>
    import Article from "./Article.vue";
    export default {
        name: "Body",
        components: { Article },
        data() {
            return {
                articles: [{
                  "title": "Networked holistic methodology",
                  "subText": "Maecenas ut massa quis augue luctus tincidunt. Nulla mollis molestie lorem. Quisque ut erat.\n\nCurabitur gravida nisi at nibh. In hac habitasse platea dictumst. Aliquam augue quam, sollicitudin vitae, consectetuer eget, rutrum at, lorem.\n\nInteger tincidunt ante vel ipsum. Praesent blandit lacinia erat. Vestibulum sed magna at nunc commodo placerat.",
                  "tags": ["vue", "javascript", "frontend"],
                  "postTime": "3/1/2018",
                  "gender": "USD",
                  "ip_address": "PHP"
                    }, {
                      "title": "Multi-lateral eco-centric service-desk",
                      "subText": "Nam ultrices, libero non mattis pulvinar, nulla pede ullamcorper augue, a suscipit nulla elit ac nulla. Sed vel enim sit amet nunc viverra dapibus. Nulla suscipit ligula in lacus.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "12/20/2017",
                      "gender": "PEN",
                      "ip_address": "CNY"
                    }, {
                      "title": "Right-sized multi-state solution",
                      "subText": "In hac habitasse platea dictumst. Morbi vestibulum, velit id pretium iaculis, diam erat fermentum justo, nec condimentum neque sapien placerat ante. Nulla justo.\n\nAliquam quis turpis eget elit sodales scelerisque. Mauris sit amet eros. Suspendisse accumsan tortor quis turpis.\n\nSed ante. Vivamus tortor. Duis mattis egestas metus.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "1/12/2018",
                      "gender": "CNY",
                      "ip_address": "CNY"
                    }, {
                      "title": "Advanced reciprocal info-mediaries",
                      "subText": "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Vivamus vestibulum sagittis sapien. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.\n\nEtiam vel augue. Vestibulum rutrum rutrum neque. Aenean auctor gravida sem.\n\nPraesent id massa id nisl venenatis lacinia. Aenean sit amet justo. Morbi ut odio.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "1/20/2018",
                      "gender": "IRR",
                      "ip_address": "EUR"
                    }, {
                      "title": "Fundamental directional help-desk",
                      "subText": "Morbi porttitor lorem id ligula. Suspendisse ornare consequat lectus. In est risus, auctor sed, tristique in, tempus sit amet, sem.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "5/6/2018",
                      "gender": "RUB",
                      "ip_address": "EUR"
                    }, {
                      "title": "Inverse didactic success",
                      "subText": "Mauris enim leo, rhoncus sed, vestibulum sit amet, cursus id, turpis. Integer aliquet, massa id lobortis convallis, tortor risus dapibus augue, vel accumsan tellus nisi eu orci. Mauris lacinia sapien quis libero.\n\nNullam sit amet turpis elementum ligula vehicula consequat. Morbi a ipsum. Integer a nibh.\n\nIn quis justo. Maecenas rhoncus aliquam lacus. Morbi quis tortor id nulla ultrices aliquet.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "4/5/2018",
                      "gender": "EUR",
                      "ip_address": "HRK"
                    }, {
                      "title": "Reverse-engineered composite framework",
                      "subText": "Praesent id massa id nisl venenatis lacinia. Aenean sit amet justo. Morbi ut odio.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "3/14/2018",
                      "gender": "XOF",
                      "ip_address": "ALL"
                    }, {
                      "title": "Up-sized global internet solution",
                      "subText": "Morbi non lectus. Aliquam sit amet diam in magna bibendum imperdiet. Nullam orci pede, venenatis non, sodales sed, tincidunt eu, felis.\n\nFusce posuere felis sed lacus. Morbi sem mauris, laoreet ut, rhoncus aliquet, pulvinar sed, nisl. Nunc rhoncus dui vel sem.\n\nSed sagittis. Nam congue, risus semper porta volutpat, quam pede lobortis ligula, sit amet eleifend pede libero quis orci. Nullam molestie nibh in lectus.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "3/29/2018",
                      "gender": "PHP",
                      "ip_address": "EUR"
                    }, {
                      "title": "Enterprise-wide motivating open architecture",
                      "subText": "Proin eu mi. Nulla ac enim. In tempor, turpis nec euismod scelerisque, quam turpis adipiscing lorem, vitae mattis nibh ligula nec sem.\n\nDuis aliquam convallis nunc. Proin at turpis a pede posuere nonummy. Integer non velit.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "10/20/2017",
                      "gender": "USD",
                      "ip_address": "USD"
                    }, {
                      "title": "Focused regional analyzer",
                      "subText": "Phasellus sit amet erat. Nulla tempus. Vivamus in felis eu sapien cursus vestibulum.\n\nProin eu mi. Nulla ac enim. In tempor, turpis nec euismod scelerisque, quam turpis adipiscing lorem, vitae mattis nibh ligula nec sem.\n\nDuis aliquam convallis nunc. Proin at turpis a pede posuere nonummy. Integer non velit.",
                      "tags": ["vue", "javascript", "frontend"],
                      "postTime": "11/29/2017",
                      "gender": "AFN",
                      "ip_address": "EUR"
                    }]
            }
        },
        created() {
                // place code that will be fetching the articles from api here

                // const apiResponse = await fetch("/articles");
                // const articles = await apiResponse.json();
                // this.articles = aricles;

                // code above wont work, just pseudocode
            }
    }
</script>