<template>
    <div class="contact">
        <ul class="contact__list">
            <li class="contact__item">
                <a href="https://www.linkedin.com/in/tian-shao-113947104/" target="_blank" class="contact__link contact__link--linkedin">
                    <span class="contact__label">LinkedIn</span>  <font-awesome-icon :icon="['fab', 'linkedin']" />
                </a>
            </li>
            <li class="contact__item">
                <a href="https://github.com/zhutoutoutousan" target="_blank" class="contact__link contact__link--github">
                    <span class="contact__label">GitHub</span> <font-awesome-icon :icon="['fab', 'github']" />
                </a>
            </li>
            <li class="contact__item">
                <a href="mailto:stupidpieceofshit@126.com" target="_blank" class="contact__link contact__link--email">
                    <span class="contact__label">Email</span> <font-awesome-icon :icon="['far', 'envelope']" />
                </a>
            </li>
            <li class="contact__item">
                <a href="" target="_blank" class="contact__link contact__link--resume">
                    <span class="contact__label">Resume</span> <font-awesome-icon :icon="['fas', 'portrait']" />
                </a>
            </li>                                    
        </ul>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    .contact {
        position: absolute;
    }
</style>