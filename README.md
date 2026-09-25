VEER CARE — SIH 2026
Predictive Personnel Welfare System

VEER CARE is a welfare-support system for uniformed personnel. It combines operational information with voluntary wellness inputs to identify meaningful changes in personnel well-being and help welfare officers provide timely support.

The system looks at changes in a person's workload, duty patterns, leave, deployment and voluntary wellness information over time.
Instead of depending on one assessment or one score, VEER CARE builds a personal baseline and looks for meaningful changes from that baseline.
The flow is:
Personnel Data → Personal Baseline → Change Detection → Risk Insight → Human Review → Welfare Support

-> Main Users
Personnel
• Complete voluntary wellness check-ins
• View their own well-being trends
• Request welfare support
• Talk to the VEER companion

Welfare Officer
• Review personnel who may need attention
• See risk trends and contributing factors
• Decide and record appropriate welfare interventions

Commander
• View unit-level welfare and workload trends
• Understand broader operational patterns
• No unnecessary access to individual sensitive information

HR
• View workforce-level trends related to duty, leave, deployment and welfare


-> Technical Overview

Frontend
Next.js · TypeScript · Tailwind CSS · Vercel

Backend
Python · FastAPI · SQLAlchemy · SQLite

ML
Python · Pandas · Scikit-learn · XGBoost


Frontend
The frontend contains the role-based interfaces and user interaction layer of VEER CARE.

Main areas include:
• Personnel dashboard
• Welfare Officer dashboard
• Commander dashboard
• HR dashboard
• Wellness assessments
• Risk and trend views
• VEER companion
Frontend architecture and details:
→ FRONTEND.md

Backend
The backend handles the APIs, authentication, database models, data processing and ML services.

Main parts include:
• API routes
• Authentication
• Database models
• Wellness and operational data
• ML prediction services
• Welfare interventions
Backend architecture and details:
→ BACKEND.md


Machine Learning
The backend currently contains separate model components for:
• Welfare
• PSS
• Burnout
• Strain
The ML output is used as a decision-support signal. Final welfare decisions remain with the authorised human reviewer.

Privacy
VEER CARE is designed around welfare support rather than disciplinary use.
The system uses role-based access and limits sensitive information according to the user's role. Personnel-level information is kept separate from the aggregate views provided to commanders and leadership.

-> Project Repositories
Frontend Repository
https://github.com/topCodegeek/veercare-frontend-sih

Backend Repository
https://github.com/topCodegeek/veercare-backend-sih

Smart India Hackathon 2026
Problem Statement: 26186
Theme: MedTech / BioTech / HealthTech
