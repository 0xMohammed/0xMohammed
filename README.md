# Hi! I'm Mohammed 👋

```tsx
import React, { useState } from "react";

const AboutMe = () => {
  const [state, setState] = useState({
    name: "Mohammed Alharbi",
    age: 21,
    location: "Saudi Arabia",
    hobbies: ["Programming", "Swimming"],
    languages: ["Arabic", "English"],
    techStack: [
      "HTML", "CSS", "JavaScript", "TypeScript",
      "React", "Next.js", "Vite", "Tailwind",
      "Express", "NestJS", "MySQL", "Python"
    ]
  });

  return (
    <div style={{ fontFamily: "Consolas, monospace", background: "#282c34", color: "#61dafb", padding: "2rem", borderRadius: "10px", maxWidth: "600px", margin: "auto" }}>
      <h1>About Me</h1>
      <p>
        Hello! I'm <strong>{state.name}</strong>, a {state.age}-year-old developer based in {state.location}.
      </p>
      <p>
        I enjoy: <em>{state.hobbies.join(", ")}</em>.
      </p>
      <p>
        Languages I speak: <em>{state.languages.join(", ")}</em>.
      </p>
      <p>
        Tech stack: <em>{state.techStack.join(", ")}</em>.
      </p>
    </div>
  );
};

export default AboutMe;
```
