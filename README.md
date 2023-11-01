# CSS variables with Javascript

Changing the image nature by css variable using javascript

- Html structure with image and input type range for blur and spacing with border color 
- with css work with script 

```
function handleUpdate() {
  const suffix = this.dataset.sizing || '';
  document.documentElement.style.setProperty(`--${this.name}`, this.value + suffix);
}

inputs.forEach(input => input.addEventListener('change', handleUpdate));
inputs.forEach(input => input.addEventListener('mousemove', handleUpdate));
```