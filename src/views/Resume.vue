<script setup>
import avatarUrl from '@/assets/avatar/avatar.jpg'
</script>

<template>
  <article class="resume-wrapper text-center position-relative">
    <div class="resume-wrapper-inner mx-auto text-start" style="display: flex; justify-content: end">
      <a style="text-decoration: none;" href="https://raw.githubusercontent.com/EjazEkay/portfolio/main/resume.pdf"
        ><button class="btn-green" style="margin-bottom: 24px; width: 160px; border-radius: 4px">
          Download PDF
        </button></a
      >
    </div>
    <div class="resume-wrapper-inner mx-auto text-start bg-white shadow-lg">
      <header class="resume-header pt-4 pt-md-0">
        <div class="row">
          <div class="col-block col-md-auto resume-picture-holder text-center text-md-start">
            <el-avatar style="border-radius: 0" :size="220" shape="square" :src="avatarUrl" alt="Avatar"> </el-avatar>
          </div>
          <!--//col-->
          <div class="col">
            <div class="row p-4 justify-content-center justify-content-md-between">
              <div class="primary-info col-auto">
                <h1 class="name mt-0 mb-1 text-white text-uppercase text-uppercase">Ijaz Ul Haq</h1>
                <div class="title mb-3">MEVN Stack Developer</div>
                <ul class="list-unstyled">
                  <li class="mb-2">
                    <a class="text-link" href="#"
                      ><i class="far fa-envelope fa-fw me-2" data-fa-transform="grow-3"></i>ejazulhaq8281@gmail.com</a
                    >
                  </li>
                  <li>
                    <a class="text-link" href="#"
                      ><i class="fas fa-mobile-alt fa-fw me-2" data-fa-transform="grow-6"></i>+923055958063</a
                    >
                  </li>
                </ul>
              </div>
              <!--//primary-info-->
              <div class="secondary-info col-auto mt-2">
                <ul class="resume-social list-unstyled">
                  <li class="mb-3">
                    <a class="text-link" href="https://github.com/EjazEkay"
                      ><span class="fa-container text-center me-2"><i class="fab fa-github-alt fa-fw"></i></span
                      >EjazEkay</a
                    >
                  </li>
                  <li class="mb-3">
                    <a class="text-link" href="https://codepen.io/Ijaz-Ul-Haq"
                      ><span class="fa-container text-center me-2"><i class="fab fa-codepen fa-fw"></i></span
                      >Ijaz-Ul-Haq</a
                    >
                  </li>
                </ul>
              </div>
              <!--//secondary-info-->
            </div>
            <!--//row-->
          </div>
          <!--//col-->
        </div>
        <!--//row-->
      </header>
      <div class="resume-body p-5">
        <section class="resume-section summary-section mb-5">
          <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Career Summary</h2>
          <div class="resume-section-content">
            <p class="mb-0">
              I am a skilled Full Stack Developer with expertise in Node.js and Vue.js, along with experience in Python. Over the past 4 years, I have built and maintained various web applications, demonstrating my ability to handle both front-end and back-end development tasks effectively.
            </p>
          </div>
        </section>
        <!--//summary-section-->
        <div class="row">
          <div class="col-lg-3" style="width: 100%">
            <section class="resume-section skills-section mb-5">
              <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Skills &amp; Tools</h2>
              <div class="resume-section-content">
                <div class="resume-skill-item">
                  <h4 class="resume-skills-cat font-weight-bold">Frontend</h4>
                  <ul class="list-unstyled mb-4">
                    <li class="mb-2">
                      <div class="resume-skill-name">Vue</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 82%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">React</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 55%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">JavaScript</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 90%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>

                    <li class="mb-2">
                      <div class="resume-skill-name">HTML/CSS/SASS</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 96%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>
                  </ul>
                </div>
                <!--//resume-skill-item-->

                <div class="resume-skill-item">
                  <h4 class="resume-skills-cat font-weight-bold">Backend</h4>
                  <ul class="list-unstyled">
                    <li class="mb-2">
                      <div class="resume-skill-name">Node.js/Express/Fastify</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 90%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>
                    <li class="mb-2">
                      <div class="resume-skill-name">Python/Django</div>
                      <div class="progress resume-progress custom-color">
                        <div
                          class="progress-bar theme-progress-bar-dark"
                          role="progressbar"
                          style="width: 55%"
                          aria-valuenow="25"
                          aria-valuemin="0"
                          aria-valuemax="100"
                        ></div>
                      </div>
                    </li>
                  </ul>
                </div>
                <!--//resume-skill-item-->

                <div class="resume-skill-item">
                  <h4 class="resume-skills-cat font-weight-bold">Others</h4>
                  <ul class="list-inline">
                    <li class="list-inline-item">
                      <span class="badge badge-light">Figma</span>
                    </li>
                    <li class="list-inline-item">
                      <span class="badge badge-light">Code Review</span>
                    </li>
                    <li class="list-inline-item">
                      <span class="badge badge-light">Git</span>
                    </li>
                    <li class="list-inline-item">
                      <span class="badge badge-light">Wireframing</span>
                    </li>
                    <li class="list-inline-item">
                      <span class="badge badge-light">Agile Methodologies</span>
                    </li>
                  </ul>
                </div>
                <!--//resume-skill-item-->
              </div>
              <!--resume-section-content-->
            </section>
            <!--//skills-section-->
            <section class="resume-section education-section mb-5">
              <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Education</h2>
              <div class="resume-section-content">
                <ul class="list-unstyled">
                  <li class="mb-2">
                    <div class="resume-degree font-weight-bold">BSc Computer Science</div>
                    <div class="resume-degree-org">Qurtuba University</div>
                    <div class="resume-degree-time">2020 - 2024</div>
                  </li>
                </ul>
              </div>
            </section>
            <!--//education-section-->
            <section class="resume-section language-section mb-5">
              <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Language</h2>
              <div class="resume-section-content">
                <ul class="list-unstyled resume-lang-list">
                  <li class="mb-2">
                    <span class="resume-lang-name font-weight-bold">Urdu</span>
                    <small class="text-muted font-weight-normal">(Native)</small>
                  </li>
                  <li class="mb-2 align-middle">
                    <span class="resume-lang-name font-weight-bold">English</span>
                    <small class="text-muted font-weight-normal">(Professional)</small>
                  </li>
                </ul>
              </div>
            </section>
            <!--//language-section-->
            <section class="resume-section interests-section mb-5">
              <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">Interests</h2>
              <div class="resume-section-content">
                <ul class="list-unstyled">
                  <li class="mb-1">Video Games</li>
                </ul>
              </div>
            </section>
            <!--//interests-section-->
          </div>
        </div>
        <!--//row-->
      </div>
      <!--//resume-body-->
    </div>
  </article>
</template>

<style scoped>
@import url('@/assets/css/pillar-1.css');
.resume-wrapper {
  font-family: roboto;
  background-color: #fff;
  line-height: 1.5;
}
.custom-color {
  background-color: #e9ecef;
}
</style>
