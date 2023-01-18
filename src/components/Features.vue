<script setup lang="ts">
import WelcomeItem from "./FeatureItem.vue";
import SupportIcon from "./icons/IconSupport.vue";
import {
  PencilSquareIcon,
    BoltIcon,
    BookOpenIcon,
    ServerStackIcon,
    HeartIcon
} from "@heroicons/vue/20/solid";
</script>

<template>
  <div class="flex flex-wrap justify-center">
    <WelcomeItem>
      <template #icon>
        <PencilSquareIcon class="w-5" />
      </template>
      <template #heading>Markdown Based</template>

      <div>
        Notes are written in
        <a class="welcomeLink" href="https://en.wikipedia.org/wiki/Markdown">Markdown</a>.
        A widely used markup language to add formatting to any text document!
        <br><br>
        An Example:
        <ul>
          <li>To write <b>bold</b> text, you type <code>**bold**</code> </li>
          <li>To write <em>italic</em> text, you type <code>*italics*</code> or <code>_italics_</code> </li>
        </ul>
      </div>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <BoltIcon class="w-5" />
      </template>
      <template #heading>Real time Collaboration</template>
      <div>
        Changes are saved on the fly, edit on your desktop, laptop, smartphone, or all of them at once!
        <br><br>
        Collaboration features are currently in development. Share a note for public viewing, or collaborate with a lot of people on one!
      </div>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <BookOpenIcon class="w-5 " />
      </template>
      <template #heading>Open Source</template>
      <div>
        Curious about the code? Interested in being part of the development? Or are you just procrastinating? Then check out the
        <a class="welcomeLink" href="https://github.com/rewelcabiles/current">Github Repository</a>! <br> <br> A caveat, while <em>Currently Notes</em> is
        Open Source, we currently only allow users to self host their own versions of Currently Notes for their individual use only. No commercial use for now.
      </div>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <ServerStackIcon class="w-5" />
      </template>
      <template #heading>Hosting Solutions</template>
      <div>
        Right now using <em>Currently Notes</em> hosted by us is completely free while it is in development.
        Though in the future monetization is inevitable.
        We will allow anyone to use the source code and host their own private instance of <em>Currently Notes</em> for their own <b><em>personal & non-commercial</em></b> use however.
        Technical guide on how to do so is currently pending.
      </div>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <HeartIcon class="w-5" />
      </template>
      <template #heading>Support Currently!</template>

      Running the servers costs money, and I'm currently doing this for free. Help offset the costs by
      <a href="https://www.paypal.com/donate/?hosted_button_id=MB2JLEBAH7SPJ" target="_blank" rel="noopener" class="welcomeLink">donating to my paypal!</a>
      <br>
      Cant afford to donate but still want to help out? You can help by finding bugs and reporting them on the Github Repository, or by providing feedback in general!

    </WelcomeItem>
  </div>
</template>

<style scoped>
.welcomeLink {
  @apply text-zinc-50 font-mono font-extralight   transition-all underline
}

li {
  @apply font-mono py-1
}

code {
  @apply font-mono bg-zinc-200 text-zinc-700 text-sm p-1
}

</style>