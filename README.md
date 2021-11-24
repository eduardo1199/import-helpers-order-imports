# import-helpers-order-imports


 rules: {
    'no-unused-vars': 'off',
    '@typescript-eslint/no-unused-vars': 'error',
    'import-helpers/order-imports': [
      'warn',
      { 
          newlinesBetween: 'always',
          groups: [
              '/^react/',
              'module',
              '/^@/',
              '/^hooks/',
              '/^services/',
              '/^models/',
              '/^utils/',
              '/^pages/',
              '/^components/',
              '/^./components/',
              '/^./state/',
              '/^./utils/',
              ['parent', 'sibling', 'index'],
          ],
          alphabetize: { ignoreCase: true },
      }
    ],
  },
