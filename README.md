# Personal-Portfolio-Creator
Since everything is being digitalized so one of the most effective of presenting yourself is through your Personal Portfolio Website. Hence, this project/website aims to provide users a with a simple and efficient platform to create professional resumes . By leveraging technologies like HTML,CSS, PHP. 

import React from 'react';
import { FaStar, FaBook, FaBriefcase, FaBolt, FaRegSmile, FaUsers, FaGraduationCap, FaLaptopCode } from 'react-icons/fa';

const highlights = [
  {
    icon: <FaStar />,
    title: 'Dual Purpose',
    description: (
      <>
        Your website serves as both your <strong>personal portfolio</strong> 🌟 and a practical <strong>guide</strong> 📖 for users to create their own. This hands-on demonstration provides tangible value.
      </>
    ),
  },
  {
    icon: <FaBriefcase />,
    title: 'Instant Resume Generation',
    description: (
      <>
        Users can effortlessly craft a <strong>professional resume</strong> 💼, saving them valuable time and effort.
      </>
    ),
  },
  {
    icon: <FaBolt />,
    title: 'Efficiency & Quality',
    description: (
      <>
        The platform is engineered for <strong>speed</strong> ⚡ without compromising the <strong>professionalism</strong> or <strong>quality</strong> ⭐ of the output.
      </>
    ),
  },
  {
    icon: <FaRegSmile />,
    title: 'User-Centric Design',
    description: (
      <>
        With an <strong>intuitive interface</strong>, your tool is easy to navigate and use 👍, making it accessible to a wide audience.
      </>
    ),
  },
  {
    icon: <FaUsers />,
    title: 'Broad Appeal',
    description: (
      <>
        This makes your platform an ideal resource for <strong>job seekers</strong> 🎯, <strong>students</strong> 🎓, and <strong>professionals</strong> 🧑‍💻 aiming to present their credentials concisely and effectively.
      </>
    ),
  },
];

export default function ProjectHighlights() {
  return (
    <section className="project-highlights">
      <h2>Project Highlights ✨</h2>
      <ul>
        {highlights.map((item, idx) => (
          <li key={idx} className="highlight-item">
            <span className="highlight-icon">{item.icon}</span>
            <div className="highlight-content">
              <h3>{item.title}</h3>
              <p>{item.description}</p>
            </div>
          </li>
        ))}
      </ul>
      <style jsx>{`
        .project-highlights {
          background: #f9f9fc;
          border-radius: 16px;
          padding: 2rem 1.5rem;
          box-shadow: 0 2px 8px rgba(0,0,0,0.06);
          max-width: 800px;
          margin: 2rem auto;
        }
        .project-highlights h2 {
          text-align: center;
          margin-bottom: 1.5rem;
        }
        .highlight-item {
          display: flex;
          align-items: flex-start;
          gap: 1rem;
          margin-bottom: 1.2rem;
        }
        .highlight-icon {
          font-size: 2rem;
          color: #6c63ff;
          flex-shrink: 0;
        }
        .highlight-content h3 {
          margin: 0 0 0.3rem 0;
          font-size: 1.1rem;
        }
        .highlight-content p {
          margin: 0;
          font-size: 1rem;
        }
        @media (max-width: 600px) {
          .project-highlights {
            padding: 1rem 0.5rem;
          }
          .highlight-item {
            flex-direction: column;
            align-items: flex-start;
          }
        }
      `}</style>
    </section>
  );
}
