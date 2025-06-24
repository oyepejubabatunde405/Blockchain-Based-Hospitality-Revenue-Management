# Blockchain-Based Hospitality Revenue Management

A comprehensive smart contract system built on the Stacks blockchain using Clarity for managing hospitality revenue operations. This system provides verification, pricing optimization, occupancy forecasting, revenue tracking, and market analysis capabilities for hotels and hospitality businesses.

## 🏨 Overview

This project implements a decentralized revenue management system that enables:

- **Revenue Manager Verification**: Secure validation and management of hospitality revenue managers
- **Pricing Optimization**: Dynamic room pricing based on demand, seasonality, and occupancy factors
- **Occupancy Forecasting**: Predictive analytics for occupancy rates using historical data
- **Revenue Tracking**: Comprehensive revenue performance monitoring and target tracking
- **Market Analysis**: Competitive intelligence and market condition analysis

## 🚀 Features

### Revenue Manager Verification Contract
- Verify and manage hospitality revenue managers
- Role-based access control for all system operations
- Manager profile management with hotel associations
- Verification status tracking and revocation capabilities

### Pricing Optimization Contract
- Dynamic pricing algorithms based on multiple factors
- Base price management per hotel
- Demand, seasonal, and occupancy multipliers
- Real-time optimized price calculations

### Occupancy Forecasting Contract
- Historical occupancy data storage and management
- Simple moving average forecasting algorithm
- Current occupancy tracking
- 12-month historical data analysis

### Revenue Tracking Contract
- Daily and monthly revenue recording
- Revenue target setting and achievement tracking
- Performance metrics calculation (ADR, RevPAR)
- Target achievement percentage calculations

### Market Analysis Contract
- Competitive market data management
- Price positioning analysis
- Market trend tracking
- Comprehensive market scoring system

## 📋 Prerequisites

- Stacks blockchain development environment
- Clarity smart contract knowledge
- Node.js and npm for testing
- Vitest for running tests

## 🛠️ Installation

1. Clone the repository:
   \`\`\`bash
   git clone <repository-url>
   cd hospitality-revenue-management
   \`\`\`

2. Install dependencies:
   \`\`\`bash
   npm install
   \`\`\`

3. Run tests:
   \`\`\`bash
   npm test
   \`\`\`

## 📁 Project Structure

\`\`\`
contracts/
├── revenue-manager-verification.clar  # Manager verification and access control
├── pricing-optimization.clar          # Dynamic pricing algorithms
├── occupancy-forecasting.clar         # Occupancy prediction system
├── revenue-tracking.clar              # Revenue monitoring and targets
└── market-analysis.clar               # Market intelligence and analysis

tests/
├── revenue-manager-verification.test.js
├── pricing-optimization.test.js
├── occupancy-forecasting.test.js
├── revenue-tracking.test.js
└── market-analysis.test.js
\`\`\`

## 🔧 Usage

### 1. Manager Verification
First, verify a revenue manager:
\`\`\`clarity
(contract-call? .revenue-manager-verification verify-manager
'SP1234... "John Doe" "HOTEL001")
\`\`\`

### 2. Set Base Pricing
Configure base room pricing:
\`\`\`clarity
(contract-call? .pricing-optimization set-base-price "HOTEL001" u15000)
\`\`\`

### 3. Update Occupancy Data
Record current occupancy:
\`\`\`clarity
(contract-call? .occupancy-forecasting update-occupancy-data "HOTEL001" u75)
\`\`\`

### 4. Track Revenue
Record daily revenue:
\`\`\`clarity
(contract-call? .revenue-tracking record-daily-revenue "HOTEL001" "2024-01-15" u25000)
\`\`\`

### 5. Market Analysis
Update market conditions:
\`\`\`clarity
(contract-call? .market-analysis update-market-data "HOTEL001" u5 u12000 u70 u85)
\`\`\`

## 🧪 Testing

The project includes comprehensive tests for all contracts:

\`\`\`bash
# Run all tests
npm test

# Run specific contract tests
npm test -- revenue-manager-verification
npm test -- pricing-optimization
npm test -- occupancy-forecasting
npm test -- revenue-tracking
npm test -- market-analysis
\`\`\`

## 🔐 Security Features

- **Access Control**: Only verified revenue managers can modify data
- **Data Validation**: Input validation for all contract functions
- **Error Handling**: Comprehensive error codes and handling
- **Immutable Records**: Blockchain-based data integrity

## 📊 Key Metrics Tracked

- **Revenue Performance**: Daily/monthly revenue, ADR, RevPAR
- **Occupancy Rates**: Current, historical, and forecasted occupancy
- **Pricing Optimization**: Dynamic pricing based on market conditions
- **Market Position**: Competitive analysis and market share
- **Target Achievement**: Performance against revenue targets

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests for new functionality
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support and questions:
- Create an issue in the repository
- Contact the development team
- Check the documentation for common solutions

## 🔮 Future Enhancements

- Advanced ML-based forecasting algorithms
- Integration with external market data APIs
- Mobile application for revenue managers
- Real-time dashboard and analytics
- Multi-property management capabilities
- Integration with property management systems (PMS)

