# VIORA-AI — Your Comprehensive AI Health & Fitness Companion

VIORA-AI is an advanced health, fitness, and diet companion platform. Powered by the **Google Gemini API**, it provides users with real-time, context-aware insights, AI-driven food scanning, and personalized wellness plans to elevate their lifestyle.

🔗 **Live Demo:** [https://viorafitness.vercel.app/](https://viorafitness.vercel.app/)

---

## ✨ Key Features

VIORA-AI seamlessly integrates a suite of health and wellness tools into one cohesive experience:

- 🍎 **Intelligent AI Food Scanner:** Leverages Google Gemini Vision API to analyze food images in real-time, accurately identifying meals, estimating calories, and instantly logging dietary intake.
- 🏋️ **Workout Tracking & Routines:** Explore customized workout plans, including targeted body-part selections (`BodySelector`), detailed workout tracking (`WorkoutTracker`), and progression modeling.
- 🧘 **AI Posture Coach:** Employs advanced computer vision (`@mediapipe/pose`) integrated with real-time feedback to actively monitor and correct your exercise postures, ensuring maximum safety and workout efficiency.
- 🥗 **Diet Intelligence:** Get dynamically curated diet plans (`DietPlan`) and deep dietary insights (`DietInsight`) tailored around your fitness goals and recorded daily intake.
- 😴 **Sleep Scheduler:** Comprehensive tools to build, refine, and track your nighttime routines and sleep schedules to ensure optimal recovery (`SleepSchedule`).
- 👥 **Community Integration:** Participate in fitness communities, share milestones, and engage with other dedicated users (`Community`).
- 🎙️ **Hands-Free Voice Logging:** Voice-to-text integration for frictionless meal and routine logging on the go.

---

## 🛠️ Tech Stack

VIORA-AI is built on a modern, robust web development ecosystem ensuring a smooth, scalable user experience.

| Category | Technology |
|---|---|
| **Frontend** | React 18, TypeScript |
| **Framework & Build** | Vite |
| **Styling** | Tailwind CSS |
| **UI Components** | shadcn/ui (Radix UI primitives) |
| **AI LLM Engine** | Google Gemini API (`@google/generative-ai`) |
| **Computer Vision** | MediaPipe (`@mediapipe/camera_utils`, `@mediapipe/pose`) |
| **Data Visualization**| Recharts |
| **Routing** | React Router DOM |
| **Package Manager** | npm / bun |

---

## 🤖 Google AI Integration

VIORA-AI utilizes **Google Gemini** at its core to drive smart features:
- **Generative Text (Gemini Flash/Pro):** Powers responsive conversational elements, diet plan generation, and intelligent routine adjustments tailored directly to the user's historical context.
- **Gemini Vision API:** Drives the core **Food Scanner**, actively analyzing visual data to parse ingredients and nutritional info instead of relying on manual entry. 

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ or Bun
- A **Google Gemini API Key**. Get yours at [Google AI Studio](https://aistudio.google.com).

### Installation & Setup

1. **Clone the deployment repository:**
   ```bash
   git clone https://github.com/VismayaGawriKrishnan/adoapps-main-main.git
   cd adoapps-main-main
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   bun install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory and add your API key:
   ```env
   VITE_GEMINI_API_KEY=your_gemini_api_key_here
   ```

4. **Run the local development server:**
   ```bash
   npm run dev
   ```
   Open `http://localhost:5173` to view the application in the browser!

### Building for Production
```bash
npm run build
npm run preview
```

---

## 📁 Project Structure Highlights

```
├── src/
│   ├── components/         # Reusable shadcn/ui functional components & AI Modules (e.g., AIPostureCoach)
│   ├── pages/              # Primary route views (FoodScanner, DietPlan, Workouts, SleepSchedule, etc.)
│   ├── lib/                # Utilities and core API wrapper configurations (gemini.ts)
│   ├── hooks/              # Custom application logic (theme, tracking, media processing)
│   └── main.tsx            # Application entry
├── public/                 # Static media and app icons
├── vite.config.ts          # Vite bundler configurations
└── tailwind.config.ts      # Tailwind theming and branding configurations
```

---

## 🌍 Deployment

VIORA-AI is configured for seamless deployment on Vercel. 

To deploy manually using the Vercel CLI:
```bash
npx vercel --prod
```

---

## 📄 License

This project is licensed under the MIT License.
