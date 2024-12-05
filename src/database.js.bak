import { openDB } from 'idb';

const DB_NAME = 'OstokseniDB';
const DB_VERSION = 1;
const STORE_NAMES = ['categories', 'products']; 

const initDB = async () => {
  return openDB(DB_NAME, DB_VERSION, {
    upgrade(db) {
      if (!db.objectStoreNames.contains('categories')) {
        db.createObjectStore('categories', { keyPath: 'id', autoIncrement: true });
      }
      if (!db.objectStoreNames.contains('products')) {
        db.createObjectStore('products', { keyPath: 'id', autoIncrement: true });
      }
    },
  });
};

export const getDB = async () => {
  const db = await initDB();
  return db;
};

