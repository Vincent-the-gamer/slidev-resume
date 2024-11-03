---
aspectRatio: 1/1.414
title: Vincent's Resume
---

<div class="hack" text-left>

<div text-center mt--5>
  <div font-bold font-size-40px >Vincent</div>
  <div>
    <div inline-flex items-center>
      <span pr-1><carbon-phone/></span>
      <span>12345678910</span>
    </div>
    <span mx-2>·</span>
    <div inline-flex items-center>
      <span pr-1><carbon-email /></span>
      <span>your@email.com</span>
    </div>
    <span mx-2>·</span>
    <div inline-flex items-center>
      <span pr-1><tabler-brand-github /></span>
      <a href="https://github.com/Vincent-the-gamer" target="_blank">Vincent-the-gamer</a>
    </div>
  </div>
</div>

<div mt-6 info>
  <h2 text-l mb-2 font-bold>Information</h2>
  <ul>
    <li>
        <span pr-1><carbon-home /></span>
        address: undefined
    </li>
  </ul>
</div>

<WorkExperience title="Experiences"
  :experiences="[
  { time: ['2024-01-01', '2024-02-01'], company: 'XXX Company', role: 'Frontend Dev' }
]"/>

<h2 text-l mt-5 mb-2 font-bold>SKills</h2>
<List listStyleType="none" :list="[
  `- Experience with HTML, CSS and JS/TS.`,
  `- Experience in Vue UI framework.`,
  `- Experience writing SpringBoot applications(in Java).`
]"/>

<h2 text-l mt-5 mb-2 font-bold>Projects</h2>

<div mt-5>
  <div font-bold text-2xl mb-2>
      <span pr-2><tabler-brand-github /></span>
      <a href="https://github.com/Vincent-the-gamer/cardforge" target="_blank">CardForge</a>
  </div>
  <ItemKeyValue itemValue="A HearthStone card maker."/>
  <div mb-1>
    <span text-l mt-5 mb-2 font-bold>Features: </span>
    <List :list="[
    `Multilingual UI.`,
    `You can make a HearthStone card within 1 min.`,
    `High similarity in font.`
    ]" />
  </div>
</div>

<div mt-5>
  <div font-bold text-2xl mb-2>
      <span pr-2><tabler-brand-github /></span>
      <a href="https://github.com/Vincent-the-gamer/utils" target="_blank">@vincent-the-gamer/utils</a>
  </div>
  <ItemKeyValue itemValue="An JavaScript/TypeScript tool library."/>
  <div mb-1>
    <span text-l mt-5 mb-2 font-bold>Features: </span>
    <List :list="[
    `Fully TypeScript`,
    `Can use in both browser and Node.js environment.`,
    ]" />
  </div>
</div>

<div mt-5>
  <div font-bold text-2xl mb-2>
      <span pr-2><tabler-brand-github /></span>
      <a href="https://github.com/Vincent-the-gamer/modern-html2pdf" target="_blank">modern-html2pdf</a>
  </div>
  <ItemKeyValue itemValue="Converts HTML elements to multi pages PDF."/>
  <div mb-1>
    <span text-l mt-5 mb-2 font-bold>Features: </span>
    <List :list="[
    `Support SVG, Custom fonts.`,
    `Render HTML DOM Nodes as multi pages PDF, split pages node by node`,
    `Easy to use, just call 1 function.`,
    ]" />
  </div>
</div>

<div mt-6>
  <h2 text-2xl mb-2 font-bold>About</h2>
  <List listStyleType="none" :list="[
    `- I am an open-source enthusiast and maintainer.`,
    `- I love how collaboration and knowledge sharing happens through open-source.`,
    `- I am very happy to see what I do could eventually feedback to the community and industry.`]" />
</div>

</div>
