# United Airlines Call Center Data Analysis

## Project Overview

This project was developed as part of the United Airlines Hackathon by **Team Divine**. The objective was to analyze United Airlines' call center data to improve operational efficiency, particularly focusing on Average Handle Time (AHT) and Average Speed to Answer (AST). By analyzing call data, agent performance, customer sentiment, and call transcripts, the project aims to identify key factors driving inefficiencies and propose data-driven solutions to enhance customer satisfaction.

## Table of Contents
- [Project Overview](#project-overview)
- [Data Insights](#data-insights)
- [Analysis](#analysis)
- [Modelling](#modelling)
- [Key Recommendations](#key-recommendations)
- [Conclusion](#conclusion)
- [Contributors](#contributors)

## Data Insights

Key insights were drawn from the data regarding agent efficiency, customer loyalty, and call reasons:

1. **Efficient Agents**: Agents with AHT < 11.63 minutes were considered efficient.
2. **Elite Customers**: Customers with loyalty scores > 3 were categorized as elite, and resource allocation was optimized to maintain high-quality service for them.
3. **Call Reason Analysis**:
   - High AHT contributors: Complex issues like IRROPS (Irregular Operations) and Voluntary Change.
   - High AST contributors: Issues such as Unaccompanied Minors and Travel Updates.

## Analysis

The project uses ABC Analysis (Pareto Principle) to break down call reasons contributing to high AHT and AST:
- **Class A Reasons (Top 70%)**: IRROPS, Mileage Plus, Post Flight Communications, etc.
- **Class B Reasons (Next 20%)**: Unaccompanied Minor, Schedule Change, and Seating.
- **Class C Reasons (Bottom 10%)**: Digital Support, Baggage, and Disability.

Additionally, sentiment and silence in calls were analyzed:
- **Sentiment Impact**: Calls handled with a polite tone resulted in shorter AHT (3.7 mins), while negative tones led to longer handling times.
- **Silence-Sentiment Correlation**: Longer silence periods correlated with higher AHT (0.41 correlation coefficient).

## Modelling

Using TFIDF and call transcripts, we implemented Random Forest and Logistic Regression models to predict call reasons. The Random Forest model showed a 3% accuracy improvement, with **AST** identified as the most important feature for call prediction.

## Key Recommendations

1. **Optimize Agent Performance**: Train agents to handle complex issues and escalations more effectively.
2. **IVR System Optimization**: Enhance the Interactive Voice Response (IVR) system for more efficient routing and to handle common issues like Travel Updates and Unaccompanied Minors, reducing both AHT and AST.
3. **Sentiment-Based Call Routing**: Route calls based on customer sentiment to agents with a proven track record of handling emotionally charged situations.

## Conclusion

By implementing these recommendations, United Airlines can expect a significant reduction in both AHT and AST, leading to improved customer satisfaction and operational efficiency.

## Contributors
- **Avinandan Patel**
- **Mayank Raj**

---
