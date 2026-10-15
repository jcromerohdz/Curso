# Corso Website

Bootstrap website for training courses, workshops, seminars, etc. It has a mixed design with both light and dark colors and a modern look.

<img src="./images/screen.png" />


1. En el archivo index.html crear la siguiente seccion para el carrusel y el header
```html
    <header class="header py-7 vh-100">
      <div class="container">
        <div class="row mb-5 text-center">
          <div class="col-12 text-container">
            <h1 class="display-2 text-white mt-3">
              Explore Our Training and Seminar Videos
            </h1>
            <p class="lead text-white w-75 m-auto mb-4">
                lorem:15
            </p>
            <a href="#register" class="btn btn-primary text-uppercase">
              Register
            </a>
            <a href="#discover" class="btn btn-outline-light text-uppercase">
              Discover
            </a>
          </div>
        </div>

        <div class="row">
          <div class="col-12">
            <!-- Image Slider -->
            <div id="slider" class="carousel slide" data-bs-ride="carousel">
              <div class="carousel-indicators">
                <button
                  class="active"
                  type="button"
                  data-bs-slide-to="0"
                  data-bs-target="#slider"
                  aria-current="true"
                  aria-label="Slide 1"
                ></button>
                <button
                  type="button"
                  data-bs-slide-to="1"
                  data-bs-target="#slider"
                  aria-label="Slide 2"
                ></button>
                <button
                  type="button"
                  data-bs-slide-to="2"
                  data-bs-target="#slider"
                  aria-label="Slide 3"
                ></button>
              </div>
              <div class="carousel-inner rounded-5">
                <div class="carousel-item active">
                  <img
                    src="images/header-slide-1.jpg"
                    alt=""
                    class="d-block w-100 rounded-5"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    src="images/header-slide-2.jpg"
                    alt=""
                    class="d-block w-100 rounded-5"
                  />
                </div>
                <div class="carousel-item">
                  <img
                    src="images/header-slide-3.jpg"
                    alt=""
                    class="d-block w-100 rounded-5"
                  />
                </div>
              </div>
              <!-- Buttons -->
              <button
                class="carousel-control-prev"
                type="button"
                data-bs-slide="prev"
                data-bs-target="#slider"
              >
                <span class="carousel-control-prev-icon"></span>
                <span class="visually-hidden">Previous</span>
              </button>
              <button
                class="carousel-control-next"
                type="button"
                data-bs-slide="next"
                data-bs-target="#slider"
              >
                <span class="carousel-control-next-icon"></span>
                <span class="visually-hidden">Next</span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </header>
```

2. En archivo index.html agrega la siguiente seccion de registro
```html
    <section class="register bg-primary py-6 overflow-hidden">
      <div class="container">
        <div class="row">
          <div class="col-lg-6">
            <h2>Unlock Your Potential with Engaging Content</h2>
            <p>
                lorem:10
            </p>

            <ul class="list-unstyled vstack gap-3">
              <li>
                <i class="fas fa-square"></i>
                <strong>Gain Expertise:</strong> lorem:12              </li>
              <li>
                <i class="fas fa-square"></i>
                <strong>Stay Updated:</strong> lorem:12
              </li>
              <li>
                <i class="fas fa-square"></i>
                <strong>Expand Your Network:</strong> lorem12
              </li>
            </ul>
          </div>
          <div class="col-lg-6 p-4">
            <form>
              <div class="my-4">
                <input
                  type="text"
                  class="form-control form-control-lg rounded-0 border-0"
                  placeholder="Enter name"
                />
              </div>
              <div class="my-4">
                <input
                  type="email"
                  class="form-control form-control-lg rounded-0 border-0"
                  placeholder="Enter email"
                />
              </div>
              <div class="my-4">
                <input
                  type="text"
                  class="form-control form-control-lg rounded-0 border-0"
                  placeholder="Enter phone number"
                />
              </div>
              <div class="form-check">
                <input type="checkbox" class="form-check-input" value="" />
                <label for="terms" class="form-check-label">
                  I agree to the terms and conditions
                </label>
              </div>
              <div class="d-grid mt-4">
                <button class="btn btn-outline-dark">Register</button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>
```

3. En el archivo que se encuentra en la carpeta css/styles.css agregar lo siguiente:
```css
.header {
  min-height: 1000px;
  background: linear-gradient(to bottom right, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)), url("../images/header-background.jpg") center center no-repeat;
  background-size: cover;
}

.header .slide {
  width: 70%;
  margin: 0 auto;
}

.navbar {
  transition: all 0.5s ease-in-out;
}

.invitation-bg {
  background: linear-gradient(to bottom right, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.8)), url("../images/invitation-background.jpg") center center no-repeat;
  background-size: cover;
}

@media (max-width: 992px) {
  .navbar {
    background: var(--bs-dark);
  }
  .header {
    height: 800px !important;
    min-height: 800px !important;
  }
  .header .slide {
    width: 90%;
    margin: 0 auto;
  }
  .header .text-container p {
    width: 100% !important;
    font-size: 16px;
  }
  .register {
    padding: 40px 0 !important;
  }
  .register h2 {
    text-align: center;
  }
  .summary {
    margin-top: 0 !important;
    width: 90% !important;
  }
}

```
