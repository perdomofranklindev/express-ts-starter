# Express TypeScript Starter

A robust and production-ready starter template for building Express.js applications with TypeScript.

## 🚀 Technologies

- **Node.js** (>=20.0.0) - JavaScript runtime
- **Express.js** (^4.18.2) - Web framework
- **TypeScript** (^5.3.3) - Type-safe JavaScript
- **Jest** (^29.7.0) - Testing framework
- **ESLint** (^8.57.0) - Code linting
- **Nodemon** (^3.1.0) - Development server with hot reload
- **Helmet** (^7.1.0) - Security middleware
- **CORS** (^2.8.5) - Cross-origin resource sharing
- **dotenv** (^16.5.0) - Environment variables management

## 📋 Prerequisites

- Node.js >= 20.0.0
- npm (comes with Node.js)

## 🛠️ Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd express-ts-starter
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory:
```bash
cp .env.example .env  # if you have an example file
# or create it manually
```

## 🚀 Usage

### Development

Start the development server with hot reload:
```bash
npm run dev
```

This will:
- Watch for TypeScript file changes
- Automatically restart the server
- Enable hot reloading

### Production

Build the project:
```bash
npm run build
```

Start the production server:
```bash
npm start
```

### Testing

Run tests:
```bash
npm test
```

Run tests in watch mode:
```bash
npm run test:watch
```

Generate test coverage:
```bash
npm run test:coverage
```

## 📁 Project Structure

```
express-ts-starter/
├── src/                    # Source files
│   ├── __tests__/         # Test files
│   ├── app.ts             # Express application setup
│   └── index.ts           # Application entry point
├── .eslintrc.json        # ESLint configuration
├── .gitignore            # Git ignore rules
├── tsconfig.json         # TypeScript configuration
├── jest.config.js        # Jest configuration
└── package.json          # Project dependencies and scripts

# Ignored directories (not tracked in git)
├── node_modules/         # Dependencies (ignored)
├── dist/                 # Build output (ignored)
└── coverage/            # Test coverage reports (ignored)
```

## 🔧 Available Scripts

- `npm start` - Start the production server
- `npm run dev` - Start development server with hot reload
- `npm run build` - Build the project
- `npm run clean` - Clean the build directory
- `npm run clean:install` - Clean node_modules, package-lock.json, npm cache and reinstall dependencies
- `npm run lint` - Check for linting errors
- `npm run lint:fix` - Fix automatically fixable linting errors
- `npm run lint:check` - Check for linting errors and fail if any warnings are found
- `npm test` - Run tests
- `npm run test:watch` - Run tests in watch mode
- `npm run test:coverage` - Generate test coverage

## 🔒 Security Features

- **Helmet**: Sets various HTTP headers for security
- **CORS**: Configures Cross-Origin Resource Sharing
- **Environment Variables**: Secure configuration management

## 🧪 Testing

The project uses Jest for testing. Tests are located in the `src/__tests__` directory.

Example test structure:
```typescript
describe('Your Test Suite', () => {
  it('should do something', () => {
    expect(true).toBe(true);
  });
});
```

## 📝 TypeScript Configuration

The project uses strict TypeScript configuration for better type safety:
- Strict mode enabled
- No implicit any
- Strict null checks
- Strict function types
- And more...

## 🧹 Linting

The project uses ESLint for code quality and consistency. ESLint is configured to only check the `src` directory, ignoring other folders like `dist`, `node_modules`, and `coverage`. The following commands are available:

- `npm run lint` - Check all TypeScript files in the `src` directory for linting issues
- `npm run lint:fix` - Automatically fix linting issues in the `src` directory where possible
- `npm run lint:check` - Strict check that fails if any warnings are found in the `src` directory

The ESLint configuration includes:
- `.eslintrc.json` - Main ESLint configuration file with:
  - TypeScript-specific rules
  - Best practices for Express applications
  - Code style consistency
  - Security best practices
- `.eslintignore` - Explicitly defines which files and directories to ignore:
  - Build artifacts (`dist/`, `build/`)
  - Dependencies (`node_modules/`)
  - Test coverage (`coverage/`)
  - Environment files (`.env`, `.env.*`)
  - IDE and editor files
  - Logs and cache files
  - Configuration files

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License.

## 🙏 Acknowledgments

- Express.js team for the amazing framework
- TypeScript team for the type system
- All other open-source contributors 