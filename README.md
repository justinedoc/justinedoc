# 👋 Greetings, I'm Onyiriuka Justin!

<p id="currentFocus"></p>


const profile = {
  name: "Onyiriuka Justin",
  interests: ["Cybersecurity", "Web Development"],
  currentFocus: ["Front-end Development", "Cybersecurity"],
  pronouns: "He/him",
  funFact: "Google’s name was the fruit of a spelling mistake 😂",
  contact: "justinifeanyi56@gmail.com",
  collaborate: (projectIdea) => {
    console.log(`Let's collaborate on ${projectIdea}! 🤝`);
  },
  animate: () => {
    const focusElement = document.getElementById("currentFocus");
    const focusList = profile.currentFocus;
    let currentIndex = 0;
    let currentText = "";
    let isDeleting = false;
    function animateText() {
      const speed = 200; // Typing speed in milliseconds
      currentText = isDeleting ? focusList[currentIndex].slice(0, currentText.length - 1) : focusList[currentIndex].slice(0, currentText.length + 1);
      focusElement.textContent = currentText;
      let delta = isDeleting ? 50 : 100;
      if (!isDeleting && currentText === focusList[currentIndex]) {
        delta = 2000; // Pause at the end of typing
        isDeleting = true;
      } else if (isDeleting && currentText === "") {
        isDeleting = false;
        currentIndex = (currentIndex + 1) % focusList.length;
      }
      setTimeout(animateText, delta);
    }
    animateText();
  }
};

profile.collaborate("the next big thing");
profile.animate();


As a passionate **Cybersecurity Enthusiast** and **Web Development Artisan**, I craft secure and vibrant digital experiences. 🛡️💻

## About Me
- 🌐 Crafting the web with **HTML**, **CSS**, and **JavaScript**.
- 🔒 Exploring the depths of **Cybersecurity** to fortify the digital realm.
- 📚 Currently honing my skills in **Front-End Development** and **Cybersecurity** best practices.
- 🤝 Open to collaborating on innovative projects that challenge the status quo.

## Let's Connect
- 📧 Reach out to me at justinifeanyi56@gmail.com.
- 👥 Pronouns: **He/Him**.

## Fun Facts
- ⚡ Did you know? The name 'Google' was actually a serendipitous typo! 😂
- 🎨 I believe in the power of creativity and the impact of a well-placed semicolon.

## My GitHub Stats
!Justin's GitHub stats

## Languages and Tools
![JavaScript](https://img.shields.io/badge/-JavaScript-yellow?logo=javascript&logoColor=white)
![HTML5](https://img.shields.io/badge/-HTML5-orange?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-blue?logo=css3&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white)

## Cybersecurity Corner
```javascript
// A snippet of code to remind us of the importance of cybersecurity:
function checkPasswordStrength(password) {
  const strongRegex = new RegExp('^(?=.*[a-z])(?=.*[A-Z])(?=.*[0-9])(?=.*[!@#\$%\^&\*])(?=.{8,})');
  return strongRegex.test(password);
}




<!---
justinedoc/justinedoc is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
