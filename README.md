# import-helpers-order-imports


 rules: {
    'import-helpers/order-imports': [
      'error',
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
