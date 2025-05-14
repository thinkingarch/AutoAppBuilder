import React, { useState, useEffect, useCallback } from 'react';
import { Brain, Cpu, Lightbulb, CheckCircle, Package, Zap, Settings, Users, MessageSquare, Image as ImageIcon, ShoppingCart, BarChart2, Shield, Code } from 'lucide-react';

// --- Mock Data ---
const APP_IDEAS_BANK = [
  { name: "EcoTrack", description: "A personal carbon footprint tracker with gamified challenges and community features.", category: "Sustainability", icon: <Package size={24} className="text-green-500" /> },
  { name: "MindGarden", description: "A guided meditation and mindfulness app with personalized AI-driven sessions.", category: "Wellness", icon: <Brain size={24} className="text-blue-500" /> },
  { name: "SkillSwap", description: "A platform for local skill-sharing and bartering services.", category: "Community", icon: <Users size={24} className="text-purple-500" /> },
  { name: "StoryForge", description: "An AI-assisted collaborative storytelling platform for creative writers.", category: "Creativity", icon: <Lightbulb size={24} className="text-yellow-500" /> },
  { name: "LocalEats", description: "A hyper-local food discovery app focusing on small, independent restaurants and street food vendors.", category: "Food", icon: <ShoppingCart size={24} className="text-red-500" /> },
  { name: "CodeBuddy", description: "An AI pair programmer that helps debug code and suggests improvements.", category: "Developer Tools", icon: <Code size={24} className="text-gray-500" /> }
];

const FEATURE_BANK = [
  { id: "auth", name: "User Authentication", description: "Secure login, registration, and profile management.", icon: <Users size={20} /> },
  { id: "realtime_chat", name: "Real-time Chat", description: "Instant messaging capabilities between users.", icon: <MessageSquare size={20} /> },
  { id: "push_notifications", name: "Push Notifications", description: "Alerts and updates for users.", icon: <Zap size={20} /> },
  { id: "payment_gateway", name: "Payment Gateway", description: "Integration for processing payments.", icon: <ShoppingCart size={20} /> },
  { id: "ai_assistant", name: "AI Assistant", description: "Intelligent in-app assistance or content generation.", icon: <Brain size={20} /> },
  { id: "gamification", name: "Gamification", description: "Points, badges, and leaderboards to engage users.", icon: <BarChart2 size={20} /> },
  { id: "image_upload", name: "Image Upload & Storage", description: "Allow users to upload and store images.", icon: <ImageIcon size={20} /> },
  { id: "admin_panel", name: "Admin Panel", description: "Dashboard for app management and analytics.", icon: <Settings size={20} /> },
  { id: "data_encryption", name: "Data Encryption", description: "End-to-end encryption for sensitive data.", icon: <Shield size={20} /> }
];

// --- Helper Components ---

const LoadingSpinner = () => (
  <div className="animate-spin rounded-full h-8 w-8 border-b-2 border-indigo-500"></div>
);

const ProgressBar = ({ progress }) => (
  <div className="w-full bg-gray-200 rounded-full h-2.5 dark:bg-gray-700">
    <div
      className="bg-indigo-600 h-2.5 rounded-full transition-all duration-500 ease-out"
      style={{ width: `${progress}%` }}
    ></div>
  </div>
);

// --- Main App Component ---
function App() {
  const [stage, setStage] = useState('IDLE'); // IDLE, IDEATION, SPECIFICATION, BUILDING, READY
  const [currentIdea, setCurrentIdea] = useState(null);
  const [selectedFeatures, setSelectedFeatures] = useState([]);
  const [buildProgress, setBuildProgress] = useState(0);
  const [buildLogs, setBuildLogs] = useState([]);
  const [error, setError] = useState(null);

  const getRandomItems = useCallback((arr, num) => {
    const shuffled = [...arr].sort(() => 0.5 - Math.random());
    return shuffled.slice(0, num);
  }, []);

  const handleStartInvention = () => {
    setError(null);
    setStage('IDEATION');
    setBuildLogs(['[AI Log] Initiating app invention sequence...']);
    setCurrentIdea(null);
    setSelectedFeatures([]);
    setBuildProgress(0);

    setTimeout(() => {
      const idea = getRandomItems(APP_IDEAS_BANK, 1)[0];
      setCurrentIdea(idea);
      setBuildLogs(prev => [...prev, `[AI Log] New App Concept Generated: ${idea.name} - ${idea.category}`]);
      setStage('SPECIFICATION');
    }, 2500);
  };

  useEffect(() => {
    if (stage === 'SPECIFICATION' && currentIdea) {
      setBuildLogs(prev => [...prev, `[AI Log] Analyzing requirements for ${currentIdea.name}...`]);
      setTimeout(() => {
        const numFeatures = Math.floor(Math.random() * 3) + 3; // 3 to 5 features
        const features = getRandomItems(FEATURE_BANK, numFeatures);
        setSelectedFeatures(features);
        setBuildLogs(prev => [...prev, `[AI Log] Core features identified: ${features.map(f => f.name).join(', ')}`]);
        setStage('BUILDING');
      }, 2500);
    }
  }, [stage, currentIdea, getRandomItems]);

  useEffect(() => {
    let interval;
    if (stage === 'BUILDING') {
      setBuildLogs(prev => [...prev, `[AI Log] Commencing autonomous build for ${currentIdea.name}...`]);
      const buildSteps = [
        "Initializing project structure...",
        "Setting up database schema...",
        "Generating UI components...",
        "Implementing core logic for features...",
        "Integrating APIs (mocked)...",
        "Writing unit tests (simulated)...",
        "Compiling application modules...",
        "Running security checks (simulated)...",
        "Preparing deployment package...",
        "Finalizing build..."
      ];
      let currentStep = 0;

      interval = setInterval(() => {
        setBuildProgress(prev => {
          const nextProgress = prev + 10;
          if (nextProgress <= 100) {
            if (buildSteps[currentStep]) {
                setBuildLogs(prevLogs => [...prevLogs, `[Build] ${buildSteps[currentStep]}`]);
                currentStep++;
            }
            return nextProgress;
          } else {
            clearInterval(interval);
            setStage('READY');
            setBuildLogs(prevLogs => [...prevLogs, `[AI Log] App Blueprint for '${currentIdea.name}' is ready!`]);
            return 100;
          }
        });
      }, 800); // Simulate time for each step
    }
    return () => clearInterval(interval);
  }, [stage, currentIdea]);


  const renderStageContent = () => {
    switch (stage) {
      case 'IDLE':
        return (
          <div className="text-center">
            <h2 className="text-2xl font-semibold mb-6 text-gray-700 dark:text-gray-300">Autonomous App Factory</h2>
            <p className="mb-8 text-gray-600 dark:text-gray-400">
              Welcome! Click the button below to initiate the AI-driven app invention and building process.
              The AI will conceptualize a new application and generate its blueprint.
            </p>
            <button
              onClick={handleStartInvention}
              className="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-6 rounded-lg shadow-md transition duration-150 ease-in-out transform hover:scale-105 flex items-center justify-center mx-auto"
            >
              <Zap size={20} className="mr-2" /> Start Autonomous Invention
            </button>
          </div>
        );
      case 'IDEATION':
        return (
          <div className="text-center p-6">
            <h2 className="text-2xl font-semibold mb-4 text-indigo-600 dark:text-indigo-400">Phase 1: Ideation</h2>
            <div className="flex justify-center items-center my-8">
              <LoadingSpinner />
              <p className="ml-4 text-lg text-gray-700 dark:text-gray-300">AI is brainstorming new app ideas...</p>
            </div>
            <Lightbulb size={48} className="mx-auto text-yellow-400 animate-pulse" />
          </div>
        );
      case 'SPECIFICATION':
        return (
          <div className="text-center p-6">
            <h2 className="text-2xl font-semibold mb-4 text-indigo-600 dark:text-indigo-400">Phase 2: Specification</h2>
             <div className="flex justify-center items-center my-8">
                <LoadingSpinner />
                <p className="ml-4 text-lg text-gray-700 dark:text-gray-300">AI is defining core features for '{currentIdea?.name}'...</p>
            </div>
            {currentIdea && (
              <div className="mt-4 p-4 bg-gray-100 dark:bg-gray-700 rounded-lg shadow">
                <h3 className="text-xl font-medium text-gray-800 dark:text-gray-200">Concept: {currentIdea.name}</h3>
                <p className="text-sm text-gray-600 dark:text-gray-400">{currentIdea.description}</p>
              </div>
            )}
            <Settings size={48} className="mx-auto text-blue-400 animate-spin-slow mt-6" />
          </div>
        );
      case 'BUILDING':
        return (
          <div className="p-6">
            <h2 className="text-2xl font-semibold mb-4 text-center text-indigo-600 dark:text-indigo-400">Phase 3: Autonomous Construction</h2>
            {currentIdea && <p className="text-center text-lg mb-6 text-gray-700 dark:text-gray-300">Building: <span className="font-semibold">{currentIdea.name}</span></p>}
            <div className="my-8">
              <ProgressBar progress={buildProgress} />
              <p className="text-center mt-2 text-sm text-gray-600 dark:text-gray-400">{buildProgress}% Complete</p>
            </div>
            <Cpu size={48} className="mx-auto text-green-500 mb-6" />
          </div>
        );
      case 'READY':
        if (!currentIdea) return <p className="text-red-500">Error: App idea is missing.</p>;
        return (
          <div className="p-6">
            <h2 className="text-3xl font-bold mb-6 text-center text-green-500 dark:text-green-400">
              <CheckCircle size={32} className="inline mr-2" /> App Blueprint Generated!
            </h2>
            <div className="bg-white dark:bg-gray-800 shadow-xl rounded-lg p-6">
              <div className="flex items-center mb-4">
                {currentIdea.icon}
                <h3 className="text-2xl font-semibold ml-3 text-gray-800 dark:text-gray-200">{currentIdea.name}</h3>
              </div>
              <p className="text-sm text-gray-500 dark:text-gray-400 mb-1">Category: {currentIdea.category}</p>
              <p className="text-gray-700 dark:text-gray-300 mb-6">{currentIdea.description}</p>

              <h4 className="text-xl font-semibold mb-3 text-gray-700 dark:text-gray-200">Core Features:</h4>
              <ul className="space-y-3">
                {selectedFeatures.map(feature => (
                  <li key={feature.id} className="flex items-start p-3 bg-gray-50 dark:bg-gray-700 rounded-md shadow-sm">
                    <div className="flex-shrink-0 text-indigo-500 dark:text-indigo-400 mt-1">
                      {feature.icon}
                    </div>
                    <div className="ml-3">
                      <p className="font-medium text-gray-900 dark:text-gray-100">{feature.name}</p>
                      <p className="text-sm text-gray-600 dark:text-gray-400">{feature.description}</p>
                    </div>
                  </li>
                ))}
              </ul>
              <div className="mt-8 text-center">
                <button
                  onClick={handleStartInvention}
                  className="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-6 rounded-lg shadow-md transition duration-150 ease-in-out transform hover:scale-105 flex items-center justify-center mx-auto"
                >
                  <Zap size={20} className="mr-2" /> Invent Another App
                </button>
              </div>
            </div>
          </div>
        );
      default:
        return <p>Unknown stage.</p>;
    }
  };

  return (
    <div className="min-h-screen bg-gray-100 dark:bg-gray-900 flex flex-col items-center justify-center p-4 font-sans">
      <div className="w-full max-w-3xl bg-white dark:bg-gray-800 shadow-2xl rounded-xl overflow-hidden">
        <header className="bg-indigo-700 dark:bg-indigo-800 p-6 text-white text-center">
          <h1 className="text-3xl font-bold flex items-center justify-center">
            <Brain size={36} className="mr-3" /> AI App Inventor
          </h1>
          <p className="text-indigo-200 dark:text-indigo-300 mt-1">Simulating Autonomous App Creation</p>
        </header>

        <main className="p-6 md:p-8 min-h-[400px] flex flex-col justify-center">
          {error && <p className="text-red-500 bg-red-100 dark:bg-red-900 dark:text-red-300 p-3 rounded-md mb-4">{error}</p>}
          {renderStageContent()}
        </main>

        {(stage === 'IDEATION' || stage === 'SPECIFICATION' || stage === 'BUILDING' || stage === 'READY') && (
          <div className="bg-gray-50 dark:bg-gray-700 p-4 border-t border-gray-200 dark:border-gray-600 max-h-60 overflow-y-auto">
            <h3 className="text-sm font-semibold text-gray-700 dark:text-gray-300 mb-2">AI Process Logs:</h3>
            <div className="text-xs text-gray-500 dark:text-gray-400 space-y-1">
              {buildLogs.map((log, index) => (
                <p key={index} className="font-mono">{log}</p>
              ))}
            </div>
          </div>
        )}

        <footer className="bg-gray-100 dark:bg-gray-800 border-t border-gray-200 dark:border-gray-600 p-4 text-center">
          <p className="text-xs text-gray-500 dark:text-gray-400">
            This is a conceptual simulation. Actual autonomous app development is highly complex.
          </p>
        </footer>
      </div>
       {/* Simple dark mode toggle - for demonstration, not production-ready */}
      <button 
        onClick={() => document.documentElement.classList.toggle('dark')}
        className="mt-8 p-2 bg-gray-200 dark:bg-gray-700 text-gray-800 dark:text-gray-200 rounded-full shadow-md hover:bg-gray-300 dark:hover:bg-gray-600 transition"
        title="Toggle Dark Mode"
      >
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className="lucide lucide-moon"><path d="M12 3a6 6 0 0 0 9 9 9 9 0 1 1-9-9Z"/></svg>
      </button>
    </div>
  );
}

export default App;

// Add some basic CSS for the .animate-spin-slow if not using Tailwind JIT or if it's custom
const styleSheet = document.createElement("style");
styleSheet.type = "text/css";
styleSheet.innerText = `
  .animate-spin-slow {
    animation: spin 3s linear infinite;
  }
  @keyframes spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
  body {
    font-family: 'Inter', sans-serif; /* Assuming Inter is loaded or fallback to sans-serif */
  }
`;
document.head.appendChild(styleSheet);

