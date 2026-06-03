const checkbox = document.getElementById('theme-checkbox');
const themeLink = document.getElementById('theme');

// Load saved theme or default to light
const savedTheme = localStorage.getItem('themeName') || 'light';
themeLink.setAttribute('href', `assets/css/theme-${savedTheme}.css`);

// Set checkbox state based on saved theme
checkbox.checked = savedTheme === 'dark';

// Listen for toggle
checkbox.addEventListener('change', () => {
  const themeName = checkbox.checked ? 'dark' : 'light';
  themeLink.setAttribute('href', `assets/css/theme-${themeName}.css`);
  localStorage.setItem('themeName', themeName);
});
