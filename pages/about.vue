<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="O mně"
      subtitle="Něco o mně"
      image="/uploads/untitled83_20210318074225-1-.png"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Ahoj!</h3>
          <p>
            <strong>
              <br>Jsem Rori a tohle je můj blog. 
            </strong>
          </p>
          <p>
            Házím sem nějaké svoje výtvory, jako třeba obrázky. 
          </p>

          <p>
            Mam ráda knihy. Ale ráda i píšu, <a href="/categories/kniha-na-pokra%C4%8Dov%C3%A1n%C3%AD" target="_blank">tady</a> je moje druhá kniha, kterou mám momentálně rozpracovanou. 
            <br>
            Moje první kniha se jmenuje 
            <i>
              Orio a čtvrtá včelička
            </i>. <a href="/orio.pdf" target="_blank">Tady</a> si jí můžete stáhnout a přečíst.

          </p>
          <p>
            Zakládám si YouTube kanál, na který budu házet animace k jednotlivým kapitolám. Odkazy budete nacházet na jejich koncích. Pište mi zpětnou vazbu a tak, budu ráda 😀.
          </p>
          <!-- <quote-card /> -->
          <!-- <h3>Still More Fake Content</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci
            eligendi impedit inventore ipsa laboriosam libero magnam modi odio,
            sunt temporibus. Distinctio doloremque eum magni nostrum quasi
            ratione rem repudiandae sit! Lorem ipsum dolor sit amet, consectetur
            adipisicing elit.
            <strong>Alias aut facere harum ipsam</strong> quibusdam quidem
            quisquam saepe? Alias architecto blanditiis consequatur consequuntur
            dicta ipsa iste modi provident, quod, similique veritatis.
          </p>
        </div> -->

        <!-- <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div> -->
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Poslední příspěvky
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
