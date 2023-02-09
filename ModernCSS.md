```css
clamp()
max()
min()
minmax()

@media (min-width: 576px) {
  .container {
    max-width: 540px;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 960px;
  }
}

@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}

.reaction-button {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
}

.section-header {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.section-header__title {
  flex: 1 1 400px;
}

The 400px value for the title is the custom breakpoint that will make the wrapping happen. When the title is 400px or less, it will wrap into a new line.

.c-card {
  display: flex;
  flex-wrap: wrap-reverse;
  align-items: flex-start;
}

.wrapper {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(290px, 1fr));
  grid-gap: 1rem;
}

h2 {
  font-size: clamp(1rem, 0.5rem + 2.5vw, 3rem);
}

.wrapper {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: clamp(1rem, 2vw, 24px);
}

.o-grid__item {
  container-type: inline-size;
  --horizontal: true;
}

@container (min-width: 400px) and style(--horizontal: true) {
  /*Horizontal style*/
}

```
