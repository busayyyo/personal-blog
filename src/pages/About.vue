<template>
    <div class="content-box">
        <h1 class="post-title">About me</h1>
        <div>
            <div>
                Hi there, my name is Busayo - a designer, writer, reader...xyz
                Lately I view writing as a form of design or an act of excorcism. I can't decide.
                I hope you find something in here helpful..

                Say hi on twitter <a href="https://twitter.com/busayyyo">@busayyo</a>
            </div>
            <div><img src="static/images/uploads/about-img.jpg" alt=""></div>
        </div>
        <div>
            <h2>Some side, but very important projects</h2>
            <ul>
                <li>[Podcast] <a href="">The ONE question podcast</a> I ask some impressive people just 1 question</li>
                <li>[Udemy course] <a href="">A beginner's guide to figma</a> New to Figma, definitely check it out!</li>
                <li>[Poetry publication] <a href="">Millennialpoets</a> Are you a millennial, do you write or read poetry? Join us</li>
                <li>[Iwrite] <a href="">Iwrite</a> A fellow writer who is in need of some writing challenge, check these out!</li>
                <li>[A collection of short stories] <a href="">Love in Berlin</a> I'm currently working on a collection of short stories about love and relationships in Berlin. Check out one of the stories.</li>
            </ul>
        </div>

        <div>
            <h2>Some writings elsewhere</h2>
            <ul>
                <li>[Fiction] <a href="">Birds in flight</a></li>
                <li>[Poetry] <a href="">The poem</a></li>
                <li>[Essay] <a href="">Why poetry matters</a></li>
                <li>[Musing] <a href=""></a></li>
                <li>[Design article] <a href=""></a></li>
                <li>[Design article] <a href=""></a></li>
                <li>[Design article] <a href=""></a></li>
                <li>[Dev article] <a href=""></a></li>
                <li>[Dev article] <a href=""></a></li>
            </ul>

        </div>
        
    </div>
</template>

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
</style>
