<template>
    <div class="post">
        <div class="post-title">
            <h2>{{ article.title }}</h2>
        </div>
        <div class="post-about">{{ trimAtricle(article.subText) }} ...</div>
        <div class="post-social">
            <span class="tag">{{ renderTags(article.tags) }}</span>
            <button class="button">tweet it</button>
        </div>
        <div class="post-time">
            {{ article.postTime }}
        </div>
    </div>
</template>

<style type="text/css" scoped> 
    .post {
        padding-top: 40px;
        border-top: 1px #e1e4e8 solid !important;
        margin: 30px 0 !important;
    }

    .post-about {
        width: 100% !important;
        text-align: center !important;
        font-size: 20px !important;
    }
    .post-social {
        display: inline-block !important;
        margin: 0 auto !important;
        margin-top: 10px !important
    }
    .post-title h2 {
        font-family: "Lucida Grande","Lucida Sans Unicode","Lucida Sans" !important;
        letter-spacing: -.02em;
        font-weight: bolder !important;
        letter-spacing: 0;
        font-size: 36px;
        margin-left: -2.13px;
        line-height: 1.15;
        letter-spacing: -.020em;
    }

    button {
      color: white;
      background: #005585;
      border: 0;
      width: 70px;
      height: 32px;
      cursor: pointer;
      border-radius: 2px;
      box-shadow: 1px 1px 3px 1px rgba(0, 0, 0, 0.1);
      margin: 0 0 15px 8px;
    }
</style>

<script>
    export default {
        name: "Article",
        props: ["article", "index"],
        data() {
            return {

            }
        },
        methods: {
            trimAtricle(article) {
                return article.substr(0, 140)
            },
            renderTags(tags) {
                const modifiedTags = [];
                tags.forEach(tag => modifiedTags.push(`#${tag}`))
                return modifiedTags.join(" , ")
            }
        }
    }
</script>