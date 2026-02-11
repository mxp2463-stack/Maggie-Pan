const root = document.documentElement;
const btn = document.getElementById("themeBtn");
const year = document.getElementById("year");

year.textContent = new Date().getFullYear();

const saved = localStorage.getItem("theme");
if (saved) root.setAttribute("data-theme", saved);

btn.addEventListener("click", () => {
  const current = root.getAttribute("data-theme") || "dark";
  const next = current === "dark" ? "light" : "dark";
  root.setAttribute("data-theme", next);
  localStorage.setItem("theme", next);
});
