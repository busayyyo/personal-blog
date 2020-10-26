<template>
    <Layout :show-logo="false" class="content-box">
        <h1 class="post-title">About me</h1>
        <div>
            <div>
                Hi there, my name is Busayo - a designer, writer, reader...xyz
                Lately I view writing as a form of design or an act of excorcism. I can't decide.
                I hope you find something in here helpful..

                Say hi on twitter <a href="https://twitter.com/busayyyo">@busayyo</a>
            </div>
            <div><img src="~@/static/images/uploads/about-img.jpg" alt="author's image"></div>
        </div>
        <div>
            <h2>Some side, but very important projects</h2>
            <ul>
                <li>[Podcast] <a href="">The ONE question podcast</a> - I ask some impressive people just 1 question</li>
                <li>[Udemy course] <a href="https://t.co/1W26wp7ykg?amp=1">A beginner's guide to figma</a> - New to Figma, definitely check it out!</li>
                <li>[Poetry publication] <a href="https://medium.com/millennial-poets">Millennialpoets</a> - Are you a millennial, do you write or read poetry? Join us</li>
                <li>[Iwrite] <a href="https://iwrite.today/">Iwrite</a> - I'm working on a website where anyone can take writing challenges. Join the waitlist</li>
                <li>[A collection of short stories] <a href="">Love in Berlin</a> - I'm currently working on a collection of short stories about love and relationships in Berlin. Check out one of the stories.</li>
            </ul>
        </div>

        <div>
            <h2>Some writings elsewhere</h2>
            <ul>
                <li>[Fiction] <a href="https://medium.com/@busayomi/birds-in-flight-d740aa167a1">Birds in flight</a></li>
                <li>[Poetry] <a href="https://medium.com/millennial-poets/the-poem-e14377693eeb">The poem</a></li>
                <li>[Essay] <a href="https://medium.com/millennial-poets/why-poetry-matters-57c86a072c35">Why poetry matters</a></li>
                <li>[Musing] <a href="https://medium.com/millennial-poets/o-me-o-life-1c64df6b702a"></a>O Me! O life!</li>
                 <li>[Musing/ Article] <a href="https://medium.com/@busayomi/revamping-yourself-222229ebfae6"></a>Revamping yourself</li>
                <li>[Article] <a href="https://medium.com/@busayomi/the-fascinating-notion-of-speed-learning-4343483451e3">The Fascinating Notion of Speed Learning</a></li>
                <li>[Design article] <a href="https://medium.com/@busayomi/making-accessibility-the-default-f8a9f1d8e259">Making Accessibility the Default</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-visually-impaired-people-navigate-the-web-7f9eab9d9c37">How visually impaired people navigate the web</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-to-efficiently-use-figma-community-resources-d94c909d3a69">How to efficiently use Figma community resources</a></li>
                <li>[Design article] <a href="https://uxdesign.cc/how-to-navigate-your-entry-level-ux-job-baa42c76d0f0">How to navigate your entry-level UX job</a></li>
                <li>[Dev article] <a href="https://medium.com/@busayomi/before-and-after-pseudo-elements-3fcc7928626d">Before and After Pseudo Elements</a></li>
                <li>[Dev article] <a href="https://medium.com/@busayomi/why-you-should-write-semantic-html-bd389ffda9f4">Why you should write semantic HTML</a></li>
            </ul>

        </div>
        
    </Layout>
</template>

export default {
  metaInfo: {
    title: 'About'
  }
}

<style lang="scss">
.post-title {
  padding: calc(var(--space) / 2) 0 calc(var(--space) / 2);
  text-align: center;
}

.post {

  &__header {
    width: calc(100% + var(--space) * 2);
    margin-left: calc(var(--space) * -1);
    margin-top: calc(var(--space) * -1);
    margin-bottom: calc(var(--space) / 2);
    overflow: hidden;
    border-radius: var(--radius) var(--radius) 0 0;

    img {
      width: 100%;
    }

    &:empty {
      display: none;
    }
  }

  &__content {
    h2:first-child {
      margin-top: 0;
    }

    p:first-of-type {
      font-size: 1.2em;
      color: var(--title-color);
    }

    img {
      width: calc(100% + var(--space) * 2);
      margin-left: calc(var(--space) * -1);
      display: block;
      max-width: none;
    }
  }
}

.post-comments {
  padding: calc(var(--space) / 2);

  &:empty {
    display: none;
  }
}

.post-author {
  margin-top: calc(var(--space) / 2);
}

a {
	margin: 0 .5em;
	color: #FDB310;
}
</style>
