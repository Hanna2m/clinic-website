<template>
  <div>
    <nav>
      <div class="container">
        <a href="" class="nav-logo">
          <h3>Your Doctor</h3>
        </a>

        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#specialists">Specialists</a></li>
          <li><a href="#testimonials">Testimonials</a></li>
          <li><a class="btn" href="#appointment">Make Appointment</a></li>
        </ul>

        <ul
          class="nav-items_mobile"
          :class="this.showMobileMenu ? 'open-menu' : 'close-menu'"
        >
          <li @click="showMenu"><a href="#">Home</a></li>
          <li @click="showMenu"><a href="#services">Services</a></li>
          <li @click="showMenu"><a href="#specialists">Specialists</a></li>
          <li @click="showMenu"><a href="#testimonials">Testimonials</a></li>
          <li @click="showMenu"><a class="btn" href="#appointment">Make Appointment</a></li>
        </ul>

        <button
          v-if="showMobileMenu == true"
          id="open_nav-btn"
          @click="showMenu"
        >
          <box-icon name="menu" color="#ffffff" />
        </button>
        <button
          v-if="showMobileMenu == false"
          id="close_nav-btn"
          @click="showMenu"
        >
          <box-icon name="x" color="#ffffff"></box-icon>
        </button>
      </div>
    </nav>

    <header>
      <div class="container">
        <div class="header-content">
          <h1>Complete Health Care Solutions</h1>
          <p>
            Start taking care of your health today. Advanced technologies of
            preventive medicine for your well-being.
          </p>
          <a class="btn" href="#appointment">Make Appointment</a>
        </div>
        <div class="header-image">
          <img src="../assets/fem_doc_img.jpg" alt="header image" />
        </div>
      </div>
    </header>

    <section id="services">
      <h2>Our services</h2>
      <p>Our exelent team works for you</p>
      <div class="container">
        <article>
          <i class="bx bx-user" />
          <div>
            <h4>Online Booking</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>

        <article>
          <i class="bx bx-trophy" />
          <div>
            <h4>Qualified Doctors</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>

        <article>
          <i class="bx bx-support" />
          <div>
            <h4>Privat support</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>

        <article>
          <i class="bx bx-donate-heart" />
          <div>
            <h4>Well Cared</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>

        <article>
          <i class="bx bx-first-aid" />
          <div>
            <h4>Need Emergency</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>

        <article>
          <i class="bx bxl-meta" />
          <div>
            <h4>24 Hour Service</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat
              explicabo dolor rem eligendi fugit tempore.
            </p>
          </div>
        </article>
      </div>
    </section>

    <section id="specialists">
      <h2>Our Top Specialists</h2>
      <p>Our exelent team works for you</p>
      <div class="container">
        <article>
          <div class="specialist-img">
            <img src="../assets/specialist-1.png" alt="specialist1" />
          </div>
          <div class="specialist-details">
            <h4>Dr. Annika Smith</h4>
            <p>Pediatrics Specialist</p>
          </div>
          <div class="specialist-socials">
            <a href="https://linkedin.com" target="_blank"
              ><i class="bx bxl-linkedin"
            /></a>
            <a href="https://twitter.com" target="_blank"
              ><i class="bx bxl-twitter"
            /></a>
            <a href="https://facebook.com" target="_blank"
              ><i class="bx bxl-facebook"
            /></a>
          </div>
          <a
            href="https://api.whatsapp.com/send?phone=3197010240285"
            class="specialist-whatsapp"
            target="_blank"
            ><i class="bx bxl-whatsapp"
          /></a>
        </article>

        <article>
          <div class="specialist-img">
            <img src="../assets/specialist-2.png" alt="specialist2" />
          </div>
          <div class="specialist-details">
            <h4>Dr. John Malkovich</h4>
            <p>Surgery Specialist</p>
          </div>
          <div class="specialist-socials">
            <a href="https://linkedin.com" target="_blank"
              ><i class="bx bxl-linkedin"
            /></a>
            <a href="https://twitter.com" target="_blank"
              ><i class="bx bxl-twitter"
            /></a>
            <a href="https://facebook.com" target="_blank"
              ><i class="bx bxl-facebook"
            /></a>
          </div>
          <a
            href="https://api.whatsapp.com/send?phone=3197010240285"
            class="specialist-whatsapp"
            target="_blank"
            ><i class="bx bxl-whatsapp"
          /></a>
        </article>

        <article>
          <div class="specialist-img">
            <img src="../assets/specialist-3.png" alt="specialist3" />
          </div>
          <div class="specialist-details">
            <h4>Dr. Nika Dubrowsky</h4>
            <p>Surgery Specialist</p>
          </div>
          <div class="specialist-socials">
            <a href="https://linkedin.com" target="_blank"
              ><i class="bx bxl-linkedin"
            /></a>
            <a href="https://twitter.com" target="_blank"
              ><i class="bx bxl-twitter"
            /></a>
            <a href="https://facebook.com" target="_blank"
              ><i class="bx bxl-facebook"
            /></a>
          </div>
          <a
            href="https://api.whatsapp.com/send?phone=3197010240285"
            class="specialist-whatsapp"
            target="_blank"
            ><i class="bx bxl-whatsapp"
          /></a>
        </article>

        <article>
          <div class="specialist-img">
            <img src="../assets/specialist-4.png" alt="specialist4" />
          </div>
          <div class="specialist-details">
            <h4>Dr. Michelle Morrone</h4>
            <p>Surgery Specialist</p>
          </div>
          <div class="specialist-socials">
            <a href="https://linkedin.com" target="_blank"
              ><i class="bx bxl-linkedin"
            /></a>
            <a href="https://twitter.com" target="_blank"
              ><i class="bx bxl-twitter"
            /></a>
            <a href="https://facebook.com" target="_blank"
              ><i class="bx bxl-facebook"
            /></a>
          </div>
          <a
            href="https://api.whatsapp.com/send?phone=3197010240285"
            class="specialist-whatsapp"
            target="_blank"
            ><i class="bx bxl-whatsapp"
          /></a>
        </article>
      </div>
    </section>

    <section id="testimonials">
      <h2>What Our Patients Say</h2>
      <p>Check reviews from our patients</p>

      <div class="container">
        <swiper
          :slidesPerView="1"
          :spaceBetween="30"
          :pagination="{
            clickable: true,
          }"
          :modules="modules"
          :breakpoints="{
            600: {
              slidesPerView: 2,
            },
            1024: {
              slidesPerView: 3,
            },
          }"
          class="mySwiper"
        >
          <swiper-slide>
            <article>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing
                elit.bcaecati quisquam unde eveniet libero quod nobis
                necessitatibus omnis sunt. Perspiciatis, ipsa.
              </p>
              <div class="patient">
                <div class="avatar">
                  <img src="../assets/person1.jpg" alt="patient1" />
                </div>
                <div class="patient-details">
                  <h5>Jina Markus</h5>
                  <caption>
                    Patient
                  </caption>
                </div>
              </div>
            </article>
          </swiper-slide>
          <swiper-slide>
            <article>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing
                elit.bcaecati quisquam unde eveniet libero quod nobis
                necessitatibus omnis sunt. Perspiciatis, ipsa.
              </p>
              <div class="patient">
                <div class="avatar">
                  <img src="../assets/person2.jpg" alt="patient2" />
                </div>
                <div class="patient-details">
                  <h5>Mike Simons</h5>
                  <caption>
                    Patient
                  </caption>
                </div>
              </div>
            </article>
          </swiper-slide>
          <swiper-slide>
            <article>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing
                elit.bcaecati quisquam unde eveniet libero quod nobis
                necessitatibus omnis sunt. Perspiciatis, ipsa.
              </p>
              <div class="patient">
                <div class="avatar">
                  <img src="../assets/icon_female.svg" alt="patient3" />
                </div>
                <div class="patient-details">
                  <h5>Margo Jones</h5>
                  <caption>
                    Patient
                  </caption>
                </div>
              </div>
            </article>
          </swiper-slide>
          <swiper-slide>
            <article>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing
                elit.bcaecati quisquam unde eveniet libero quod nobis
                necessitatibus omnis sunt. Perspiciatis, ipsa.
              </p>
              <div class="patient">
                <div class="avatar">
                  <img src="../assets/person4.jpeg" alt="patient4" />
                </div>
                <div class="patient-details">
                  <h5>Dina Marina</h5>
                  <caption>
                    Patient
                  </caption>
                </div>
              </div>
            </article>
          </swiper-slide>
          <swiper-slide>
            <article>
              <p>
                Lorem ipsum dolor sit, amet consectetur adipisicing
                elit.bcaecati quisquam unde eveniet libero quod nobis
                necessitatibus omnis sunt. Perspiciatis, ipsa.
              </p>
              <div class="patient">
                <div class="avatar">
                  <img src="../assets/icon_male.svg" alt="patient5" />
                </div>
                <div class="patient-details">
                  <h5>Jack Toffel</h5>
                  <caption>
                    Patient
                  </caption>
                </div>
              </div>
            </article>
          </swiper-slide>
        </swiper>
      </div>
    </section>

    <section id="appointment">
      <div class="container">
        <div class="info">
          <h2>Get An Appointment</h2>
          <p>Book online your appointment</p>
          <article>
            <div class="info-icon">
              <i class="bx bx-user" />
            </div>
            <div>
              <h4>Experienced Doctors</h4>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla
                quasi obcaecati eaque. Laudantium doloribus natus iste repellat
                molestias.
              </p>
            </div>
          </article>

          <article>
            <div class="info-icon">
              <i class="bx bx-medal" />
            </div>
            <div>
              <h4>Advanced Technology</h4>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla
                quasi obcaecati eaque. Laudantium doloribus natus iste repellat
                molestias.
              </p>
            </div>
          </article>

          <article>
            <div class="info-icon">
              <i class="bx bx-first-aid" />
            </div>
            <div>
              <h4>Emergency care</h4>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla
                quasi obcaecati eaque. Laudantium doloribus natus iste repellat
                molestias.
              </p>
            </div>
          </article>
        </div>

        <form action="https://formspree.io/f/mlevalaa" method="POST">
          <div class="form-group">
            <label for="name">Name</label>
            <input
              v-model="name"
              type="text"
              placeholder="Enter Your Name"
              name="name"
            />
          </div>
          <div class="form-group">
            <label for="email">Email</label>
            <input
              type="email"
              name="email"
              v-model="email"
              placeholder="Enter Your Email"
              required
              id="email"
            />
          </div>
          <div class="form-group">
            <label for="phone">Phone</label>
            <input
              v-model="phone"
              type="number"
              placeholder="Enter Your Phone"
              name="phone"
            />
          </div>
          <div class="form-group">
            <label for="date">Date</label>
            <input
              v-model="date"
              type="date"
              placeholder="Select a Date"
              name="date"
            />
          </div>
          <div class="form-group">
            <label for="department">Department</label>
            <select v-model="selectedDepartment" name="department" required>
              <option selected>General</option>
              <option>Pediatrics</option>
              <option>Dermatology</option>
              <option>Orthopedist</option>
            </select>
          </div>
          <div class="form-group">
            <label for="doctor">Doctor</label>
            <select v-model="selectedDoctor" name="doctor">
              <option disabled value="">Please Select a Doctor</option>
              <option
                v-for="item in doctorsFilter"
                :key="item.id"
                :value="item.name"
              >
                {{ item.name }}
              </option>
            </select>
          </div>
          <div class="form-group">
            <label for="msg">Message</label>
            <textarea
              v-model="message"
              type="text"
              placeholder="Additional Message"
              rows="6"
              name="message"
            />
          </div>
          <input type="submit" value="Submit" class="btn-primary" />
        </form>
      </div>
    </section>

    <footer>
      <div class="container">
        <article>
          <a href="#" class="footer-logo"><h3>Your Doctor</h3></a>
          <div>
            <i class="bx bx-phone" />
            <p>+4912345678</p>
          </div>
          <div>
            <i class="bx bx-envelope" />
            <p>support@yourdoctor.com</p>
          </div>
        </article>
        <article>
          <h3>Support</h3>
          <a href="#">Privacy Policy</a>
          <a href="#">Cookie Policy</a>
          <a href="#">Purchasing Policy</a>
          <a href="#">Terms & Conditions</a>
        </article>
        <article>
          <h3>Menu</h3>
          <a href="#">Home</a>
          <a href="#services">Services</a>
          <a href="#specialists">Specialists</a>
          <a href="#testimonials">Testimonials</a>
          <a href="#appointment" class="btn-primary">Get an Appointment</a>
        </article>
        <article>
          <h3>Contact Us</h3>
          <p>Press</p>
          <p>FAQs</p>
          <div class="footer-socials">
            <a href="https://linkedin.com" target="_blank"
              ><i class="bx bxl-linkedin"
            /></a>
            <a href="https://twitter.com" target="_blank"
              ><i class="bx bxl-twitter"
            /></a>
            <a href="https://facebook.com" target="_blank"
              ><i class="bx bxl-facebook"
            /></a>
          </div>
        </article>
      </div>
      <div class="copyright">
        <p>&copy; Copyright Your Doctor. All Rights Reserved</p>
      </div>
    </footer>
  </div>
</template>

<script>
import 'boxicons';
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/pagination';
import { Pagination } from 'swiper';

export default {
  name: 'Home',

  components: {
    Swiper,
    SwiperSlide,
  },

  setup() {
    return {
      modules: [Pagination],
    };
  },

  data() {
    return {
      showMobileMenu: true,
      name: '',
      phone: '',
      email: '',
      selectedDepartment: 'General',
      selectedDoctor: '',
      message: '',
      doctors: [
        {
          id: 1,
          department: 'General',
          name: 'Dr. Michelle Morrone',
        },
        {
          id: 2,
          department: 'General',
          name: 'Dr. Ann Litz',
        },
        {
          id: 3,
          department: 'General',
          name: 'Dr. Mick Hussle',
        },
        {
          id: 4,
          department: 'Pediatrics',
          name: 'Dr. Annika Smith',
        },
        {
          id: 5,
          department: 'Pediatrics',
          name: 'Dr. Luca Latto',
        },

        {
          id: 6,
          department: 'Dermatology',
          name: 'Dr. Susanna Smith',
        },
        {
          id: 6,
          department: 'Dermatology',
          name: 'Dr. Ricardo Gonsales',
        },
        {
          id: 6,
          department: 'Orthopedist',
          name: 'Dr. Ivan Moroz',
        },
        {
          id: 6,
          department: 'Orthopedist',
          name: 'Dr. Rebecca Lutz',
        },
      ],
    };
  },

  computed: {
    doctorsFilter: function () {
      const department = this.selectedDepartment;
      return this.doctors.filter(function (d) {
        return d.department == department;
      });
    },
  },

  methods: {
    showMenu() {
      this.showMobileMenu = !this.showMobileMenu;
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
