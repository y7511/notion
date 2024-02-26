# bootstrap

# BREACKPOINT

## **Core concepts**

- **Breakpoints are the building blocks of responsive design.** Use them to control when your layout can be adapted at a particular viewport or device size.
- **Use media queries to architect your CSS by breakpoint.** Media queries are a feature of CSS that allow you to conditionally apply styles based on a set of browser and operating system parameters. We most commonly use `min-width` in our media queries.
- **Mobile first, responsive design is the goal.** Bootstrap’s CSS aims to apply the bare minimum of styles to make a layout work at the smallest breakpoint, and then layers on styles to adjust that design for larger devices. This optimizes your CSS, improves rendering time, and provides a great experience for your visitors.

![Screenshot 2023-11-25 152134.png](bootstrap%20f4354c8bde0c4c48a9b72471fea9face/Screenshot_2023-11-25_152134.png)

```html
scss/_variables.scss

$grid-breakpoints: (
  xs: 0,
  sm: 576px,
  md: 768px,
  lg: 992px,
  xl: 1200px,
  xxl: 1400px
);
```

## **Media queries**

Since Bootstrap is developed to be mobile first, we use a handful of [media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries) to create sensible breakpoints for our layouts and interfaces. These breakpoints are mostly based on minimum viewport widths and allow us to scale up elements as the viewport changes.

### **Min-width**

Bootstrap primarily uses the following media query ranges—or breakpoints—in our source Sass files for our layout, grid system, and components.

```html
// Source mixins

// No media query necessary for xs breakpoint as it's effectively `@media (min-width: 0) { ... }`
@include media-breakpoint-up(sm) { ... }
@include media-breakpoint-up(md) { ... }
@include media-breakpoint-up(lg) { ... }
@include media-breakpoint-up(xl) { ... }
@include media-breakpoint-up(xxl) { ... }

// Usage

// Example: Hide starting at `min-width: 0`, and then show at the `sm` breakpoint
.custom-class {
  display: none;
}
@include media-breakpoint-up(sm) {
  .custom-class {
    display: block;
  }
}
```

[**Containers**](bootstrap%20f4354c8bde0c4c48a9b72471fea9face/Containers%20fe4d169a907e4e6f98df03123e87bf9a.md)

[Breakpoints](https://getbootstrap.com/docs/5.3/layout/breakpoints/)

# **Containers**

Containers are a fundamental building block of Bootstrap that contain, pad, and align your content within a given device or viewport.

[**Columns**](bootstrap%20f4354c8bde0c4c48a9b72471fea9face/Columns%209e47fe53786b4784bfd0ed67e0f795ba.md)

[Grid](bootstrap%20f4354c8bde0c4c48a9b72471fea9face/Grid%207708df4f9c284bbd826853af591cf4f8.md)