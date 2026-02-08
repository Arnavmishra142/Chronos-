// ==================== CONFIGURATION ====================
const CONFIG = {
    // Firebase Config - Your actual config
    FIREBASE: {
        apiKey: "AIzaSyAaTHjdBkYlYz3_wnUTQNdKdhw6yOoG4Zg",
        authDomain: "history-5799e.firebaseapp.com",
        projectId: "history-5799e",
        storageBucket: "history-5799e.firebasestorage.app",
        messagingSenderId: "988160924529",
        appId: "1:988160924529:web:175a8c7ddc723c7321f4d0",
        measurementId: "G-X70DNPFG4C"
    },
    
    WIKI_API: 'https://en.wikipedia.org/w/api.php',
    DEFAULT_IMAGE: 'https://images.unsplash.com/photo-1461360370896-922624d12aa1?w=1920&h=1080&fit=crop',
    
    FEATURED_TOPICS: [
        { id: 'aurangzeb', title: 'Aurangzeb', era: '1658 - 1707 AD', desc: 'The Last Great Mughal Emperor', image: 'https://images.unsplash.com/photo-1548013146-72479768bada?w=400&h=300&fit=crop' },
        { id: 'titanic', title: 'Titanic', era: '1912 AD', desc: 'The Unsinkable That Sank', image: 'https://images.unsplash.com/photo-1500077423678-25eead48513a?w=400&h=300&fit=crop' },
        { id: 'genghis-khan', title: 'Genghis Khan', era: '1206 - 1227 AD', desc: 'The Conqueror of Worlds', image: 'https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=400&h=300&fit=crop' },
        { id: 'cleopatra', title: 'Cleopatra', era: '69 - 30 BC', desc: 'The Last Pharaoh of Egypt', image: 'https://images.unsplash.com/photo-1566127444979-b3d2b654e3d7?w=400&h=300&fit=crop' },
        { id: 'napoleon', title: 'Napoleon Bonaparte', era: '1769 - 1821 AD', desc: 'The French Emperor', image: 'https://images.unsplash.com/photo-1555662092-3696d6c8a56d?w=400&h=300&fit=crop' },
        { id: 'world-war-2', title: 'World War II', era: '1939 - 1945 AD', desc: 'The Global Conflict', image: 'https://images.unsplash.com/photo-1550850839-8dc894ed385a?w=400&h=300&fit=crop' }
    ],
    
    // Comprehensive daily events database
    DAILY_EVENTS: {
        '01-01': [
            { title: 'Haiti Independence', year: '1804', desc: 'Haiti declares independence from France, becoming the first independent nation of Latin America.', image: 'https://images.unsplash.com/photo-1589829085413-56de8ae18c73?w=400&h=300&fit=crop', slug: 'haiti-independence' },
            { title: 'Euro Currency Introduced', year: '1999', desc: 'The Euro currency is introduced in 11 countries.', image: 'https://images.unsplash.com/photo-1580519542036-c47de6196ba5?w=400&h=300&fit=crop', slug: 'euro-introduction' }
        ],
        '01-27': [
            { title: 'Auschwitz Liberated', year: '1945', desc: 'Soviet troops liberate Auschwitz concentration camp.', image: 'https://images.unsplash.com/photo-1533613220915-609f661a6fe1?w=400&h=300&fit=crop', slug: 'auschwitz-liberation' }
        ],
        '02-08': [
            { title: 'Mary, Queen of Scots Executed', year: '1587', desc: 'Mary, Queen of Scots is executed at Fotheringhay Castle.', image: 'https://images.unsplash.com/photo-1599707367072-cd6ada2bc375?w=400&h=300&fit=crop', slug: 'mary-queen-scots' },
            { title: 'First US Weather Satellite', year: '1962', desc: 'NASA launches TIROS-1, the first successful weather satellite.', image: 'https://images.unsplash.com/photo-1446776811953-b23d57bd21aa?w=400&h=300&fit=crop', slug: 'tiros-1' }
        ],
        '03-15': [
            { title: 'Julius Caesar Assassinated', year: '44 BC', desc: 'Julius Caesar is assassinated by Roman senators.', image: 'https://images.unsplash.com/photo-1552832230-c0197dd311b5?w=400&h=300&fit=crop', slug: 'julius-caesar' }
        ],
        '04-12': [
            { title: 'First Human in Space', year: '1961', desc: 'Yuri Gagarin becomes the first human to journey into outer space.', image: 'https://images.unsplash.com/photo-1446776811953-b23d57bd21aa?w=400&h=300&fit=crop', slug: 'yuri-gagarin' }
        ],
        '05-29': [
            { title: 'Fall of Constantinople', year: '1453', desc: 'The Ottoman Empire captures Constantinople, ending the Byzantine Empire.', image: 'https://images.unsplash.com/photo-1541433075995-1c27e9d1a004?w=400&h=300&fit=crop', slug: 'constantinople' }
        ],
        '06-06': [
            { title: 'D-Day Landings', year: '1944', desc: 'Allied forces launch the largest seaborne invasion in history on the beaches of Normandy.', image: 'https://images.unsplash.com/photo-1550850839-8dc894ed385a?w=400&h=300&fit=crop', slug: 'd-day' }
        ],
        '07-04': [
            { title: 'US Independence Day', year: '1776', desc: 'The United States Declaration of Independence is adopted.', image: 'https://images.unsplash.com/photo-1603569283847-aa295f0d016a?w=400&h=300&fit=crop', slug: 'independence-day' }
        ],
        '07-20': [
            { title: 'Moon Landing', year: '1969', desc: 'Neil Armstrong becomes the first human to step onto the lunar surface.', image: 'https://images.unsplash.com/photo-1446776811953-b23d57bd21aa?w=400&h=300&fit=crop', slug: 'apollo-11' }
        ],
        '08-06': [
            { title: 'Atomic Bomb Dropped on Hiroshima', year: '1945', desc: 'The first atomic bomb is dropped, changing warfare forever.', image: 'https://images.unsplash.com/photo-1550850839-8dc894ed385a?w=400&h=300&fit=crop', slug: 'hiroshima' }
        ],
        '09-02': [
            { title: 'V-J Day', year: '1945', desc: 'Japan formally surrenders, ending World War II.', image: 'https://images.unsplash.com/photo-1550850839-8dc894ed385a?w=400&h=300&fit=crop', slug: 'vj-day' }
        ],
        '10-12': [
            { title: 'Discovery of America', year: '1492', desc: 'Christopher Columbus reaches the Americas.', image: 'https://images.unsplash.com/photo-1500077423678-25eead48513a?w=400&h=300&fit=crop', slug: 'columbus' }
        ],
        '11-09': [
            { title: 'Fall of the Berlin Wall', year: '1989', desc: 'The Berlin Wall falls, symbolizing the end of the Cold War.', image: 'https://images.unsplash.com/photo-1560264280-88b68371db39?w=400&h=300&fit=crop', slug: 'berlin-wall' }
        ],
        '12-25': [
            { title: 'Christmas Truce', year: '1914', desc: 'World War I soldiers along the Western Front cease fighting to celebrate Christmas.', image: 'https://images.unsplash.com/photo-1543589077-47d81606c1bf?w=400&h=300&fit=crop', slug: 'christmas-truce' }
        ]
    },
    
    // Default events for dates not in database
    DEFAULT_EVENTS: [
        { title: 'Moon Landing', year: '1969', desc: 'Neil Armstrong becomes the first human to step onto the lunar surface, marking a giant leap for mankind.', image: 'https://images.unsplash.com/photo-1446776811953-b23d57bd21aa?w=400&h=300&fit=crop', slug: 'apollo-11' },
        { title: 'Fall of the Berlin Wall', year: '1989', desc: 'The Berlin Wall falls, symbolizing the end of the Cold War and the reunification of Germany.', image: 'https://images.unsplash.com/photo-1560264280-88b68371db39?w=400&h=300&fit=crop', slug: 'berlin-wall' },
        { title: 'Discovery of America', year: '1492', desc: 'Christopher Columbus reaches the Americas, initiating widespread European exploration.', image: 'https://images.unsplash.com/photo-1500077423678-25eead48513a?w=400&h=300&fit=crop', slug: 'columbus' },
        { title: 'French Revolution Begins', year: '1789', desc: 'The Storming of the Bastille marks the beginning of the French Revolution.', image: 'https://images.unsplash.com/photo-1555662092-3696d6c8a56d?w=400&h=300&fit=crop', slug: 'french-revolution' },
        { title: 'Signing of Magna Carta', year: '1215', desc: 'King John signs the Magna Carta, establishing the principle that everyone is subject to the law.', image: 'https://images.unsplash.com/photo-1599707367072-cd6ada2bc375?w=400&h=300&fit=crop', slug: 'magna-carta' }
    ],
    
    // Timeline events for personalized generator
    TIMELINE_EVENTS: [
        { year: 1945, title: 'End of World War II', desc: 'The deadliest conflict in human history comes to an end.', categories: ['war'], significance: 10 },
        { year: 1947, title: 'India Gains Independence', desc: 'India becomes independent from British rule.', categories: ['empires'], significance: 9 },
        { year: 1957, title: 'Sputnik Launched', desc: 'The Soviet Union launches the first artificial satellite.', categories: ['space', 'tech'], significance: 9 },
        { year: 1961, title: 'First Human in Space', desc: 'Yuri Gagarin orbits Earth.', categories: ['space'], significance: 10 },
        { year: 1963, title: 'JFK Assassinated', desc: 'President John F. Kennedy is assassinated in Dallas.', categories: ['politics'], significance: 9 },
        { year: 1969, title: 'Moon Landing', desc: 'Neil Armstrong walks on the moon.', categories: ['space'], significance: 10 },
        { year: 1971, title: 'Microprocessor Invented', desc: 'The first commercial microprocessor is released.', categories: ['tech', 'inventions'], significance: 9 },
        { year: 1975, title: 'Vietnam War Ends', desc: 'The Vietnam War officially ends.', categories: ['war'], significance: 8 },
        { year: 1981, title: 'First Personal Computer', desc: 'IBM launches its first personal computer.', categories: ['tech', 'inventions'], significance: 9 },
        { year: 1986, title: 'Chernobyl Disaster', desc: 'The worst nuclear disaster in history occurs.', categories: ['science'], significance: 9 },
        { year: 1989, title: 'Fall of Berlin Wall', desc: 'The Cold War symbol crumbles.', categories: ['war', 'politics'], significance: 10 },
        { year: 1991, title: 'World Wide Web', desc: 'Tim Berners-Lee introduces the World Wide Web.', categories: ['tech', 'inventions'], significance: 10 },
        { year: 1997, title: 'First Cloned Mammal', desc: 'Dolly the sheep becomes the first cloned mammal.', categories: ['science'], significance: 8 },
        { year: 2001, title: 'September 11 Attacks', desc: 'Terrorist attacks change the world forever.', categories: ['war'], significance: 10 },
        { year: 2004, title: 'Facebook Launched', desc: 'Social media revolution begins.', categories: ['tech'], significance: 9 },
        { year: 2007, title: 'iPhone Released', desc: 'Smartphone era begins.', categories: ['tech', 'inventions'], significance: 10 },
        { year: 2011, title: 'Arab Spring', desc: 'Pro-democracy protests sweep the Middle East.', categories: ['politics'], significance: 8 },
        { year: 2020, title: 'COVID-19 Pandemic', desc: 'Global pandemic changes life worldwide.', categories: ['science'], significance: 10 }
    ],
    
    QUOTES: [
        { text: "Those who cannot remember the past are condemned to repeat it.", author: "George Santayana" },
        { text: "History doesn't repeat itself, but it often rhymes.", author: "Mark Twain" },
        { text: "The only thing we learn from history is that we learn nothing from history.", author: "Georg Wilhelm Friedrich Hegel" },
        { text: "History is written by the victors.", author: "Winston Churchill" },
        { text: "Study the past if you would define the future.", author: "Confucius" },
        { text: "Empires fall silently before they collapse loudly.", author: "Anonymous" },
        { text: "The farther backward you can look, the farther forward you are likely to see.", author: "Winston Churchill" },
        { text: "History is a set of lies agreed upon.", author: "Napoleon Bonaparte" }
    ],
    
    COUNTRY_TOPICS: {
        'US': ['American Revolution', 'Civil War', 'Moon Landing', 'September 11', 'Declaration of Independence'],
        'GB': ['Magna Carta', 'Industrial Revolution', 'World War II', 'British Empire', 'Winston Churchill'],
        'FR': ['French Revolution', 'Napoleon', 'Bastille Day', 'Joan of Arc', 'Louis XIV'],
        'DE': ['World War II', 'Berlin Wall', 'Otto von Bismarck', 'Protestant Reformation', 'Weimar Republic'],
        'IT': ['Roman Empire', 'Renaissance', 'Julius Caesar', 'Marco Polo', 'Christopher Columbus'],
        'RU': ['Russian Revolution', 'Stalin', 'Peter the Great', 'Cold War', 'Catherine the Great'],
        'CN': ['Great Wall of China', 'Mao Zedong', 'Silk Road', 'Qin Shi Huang', 'Opium Wars'],
        'IN': ['Indian Independence', 'Mahatma Gandhi', 'Mughal Empire', 'Indus Valley', 'British Raj'],
        'JP': ['Samurai', 'World War II', 'Meiji Restoration', 'Atomic Bomb', 'Tokugawa Shogunate'],
        'EG': ['Ancient Egypt', 'Pyramids', 'Cleopatra', 'Pharaohs', 'Rosetta Stone'],
        'BR': ['Brazilian Independence', 'Portuguese Empire', 'Slavery Abolition', 'Getulio Vargas'],
        'AU': ['Captain Cook', 'Aboriginal History', 'ANZAC', 'Eureka Rebellion', 'Federation'],
        'ZA': ['Nelson Mandela', 'Apartheid', 'Boer War', 'Shaka Zulu', 'Great Trek'],
        'CA': ['Canadian Confederation', 'War of 1812', 'Vimy Ridge', 'Terry Fox'],
        'MX': ['Aztec Empire', 'Mexican Revolution', 'Cinco de Mayo', 'Maya Civilization']
    },
    
    SUGGESTIONS: {
        'hitler': ['World War II', 'Nazi Germany', 'Holocaust', 'Stalin', 'Cold War'],
        'world-war-2': ['Hitler', 'Stalin', 'Winston Churchill', 'Holocaust', 'Atomic Bomb'],
        'napoleon': ['French Revolution', 'Waterloo', 'Josephine', 'Louis XVI', 'Napoleonic Wars'],
        'cleopatra': ['Julius Caesar', 'Mark Antony', 'Ancient Egypt', 'Pyramids', 'Pharaohs'],
        'genghis-khan': ['Mongol Empire', 'Silk Road', 'Kublai Khan', 'Marco Polo', 'Samurai'],
        'default': ['World War II', 'Ancient Egypt', 'Renaissance', 'Roman Empire', 'Industrial Revolution']
    },
    
    ERA_TOPICS: {
        ancient: ['Ancient Egypt', 'Roman Empire', 'Greek Civilization', 'Persian Empire', 'Alexander the Great'],
        medieval: ['Charlemagne', 'Viking Age', 'Crusades', 'Black Death', 'Magna Carta'],
        renaissance: ['Leonardo da Vinci', 'Michelangelo', 'Renaissance Art', 'Scientific Revolution', 'Printing Press'],
        industrial: ['Steam Engine', 'Industrial Revolution', 'Railways', 'Factory System', 'Urbanization'],
        modern: ['World War I', 'World War II', 'Cold War', 'Space Race', 'Digital Age']
    }
};

// ==================== FIREBASE INITIALIZATION ====================
let firebaseApp = null;
let firebaseAuth = null;
let firebaseDb = null;
let currentUser = null;

function initFirebase() {
    try {
        // Check if Firebase is available
        if (typeof firebase !== 'undefined') {
            // Initialize Firebase with the config
            firebaseApp = firebase.initializeApp(CONFIG.FIREBASE);
            firebaseAuth = firebase.auth();
            firebaseDb = firebase.firestore();
            
            console.log('Firebase initialized successfully');
            
            // Auth state listener
            firebaseAuth.onAuthStateChanged((user) => {
                currentUser = user;
                updateUIForAuthState();
                if (user) {
                    loadUserLibrary();
                    // Update last login time
                    firebaseDb.collection('users').doc(user.uid).update({
                        lastLogin: firebase.firestore.FieldValue.serverTimestamp()
                    }).catch(err => console.log('Error updating last login:', err));
                }
            });
            
            return true;
        }
        return false;
    } catch (error) {
        console.error('Firebase initialization error:', error.message);
        return false;
    }
}

// ==================== STATE MANAGEMENT ====================
const State = {
    library: [],
    collections: {},
    notes: [],
    currentAudio: null,
    speechSynth: window.speechSynthesis,
    isPlaying: false,
    currentUtterance: null,
    selectedInterests: [],
    currentNoteItem: null,
    currentCollectionItem: null,
    
    async addToLibrary(item, collection = null) {
        if (!this.library.find(i => i.slug === item.slug)) {
            // Add collection if specified
            if (collection) {
                item.collection = collection;
                if (!this.collections[collection]) {
                    this.collections[collection] = [];
                }
                this.collections[collection].push(item.slug);
            }
            
            // Add to local state
            this.library.push(item);
            
            // If user is logged in, save to Firestore
            if (currentUser && firebaseDb) {
                try {
                    await firebaseDb.collection('users').doc(currentUser.uid)
                        .collection('bookmarks').doc(item.slug)
                        .set({
                            ...item,
                            bookmarkedAt: firebase.firestore.FieldValue.serverTimestamp()
                        });
                } catch (error) {
                    console.error('Error saving bookmark:', error);
                }
            }
            
            this.saveLibrary();
            this.saveCollections();
            return true;
        }
        return false;
    },
    
    async removeFromLibrary(slug) {
        const item = this.library.find(i => i.slug === slug);
        if (item && item.collection) {
            this.collections[item.collection] = this.collections[item.collection].filter(s => s !== slug);
        }
        this.library = this.library.filter(i => i.slug !== slug);
        
        // If user is logged in, remove from Firestore
        if (currentUser && firebaseDb) {
            try {
                await firebaseDb.collection('users').doc(currentUser.uid)
                    .collection('bookmarks').doc(slug).delete();
            } catch (error) {
                console.error('Error removing bookmark:', error);
            }
        }
        
        this.saveLibrary();
        this.saveCollections();
    },
    
    saveLibrary() {
        localStorage.setItem('chronos_library', JSON.stringify(this.library));
        updateLibraryCount();
    },
    
    saveCollections() {
        localStorage.setItem('chronos_collections', JSON.stringify(this.collections));
    },
    
    loadCollections() {
        const stored = localStorage.getItem('chronos_collections');
        if (stored) {
            this.collections = JSON.parse(stored);
        }
    },
    
    isInLibrary(slug) {
        return this.library.some(i => i.slug === slug);
    },
    
    loadFromStorage() {
        const stored = localStorage.getItem('chronos_library');
        if (stored) {
            this.library = JSON.parse(stored);
            updateLibraryCount();
        }
        this.loadCollections();
        this.loadNotes();
    },
    
    // Notes functionality
    async addNote(note) {
        note.id = Date.now().toString();
        note.createdAt = new Date().toISOString();
        this.notes.push(note);
        this.saveNotes();
        
        if (currentUser && firebaseDb) {
            try {
                await firebaseDb.collection('users').doc(currentUser.uid)
                    .collection('notes').doc(note.id)
                    .set(note);
            } catch (error) {
                console.error('Error saving note:', error);
            }
        }
        return note;
    },
    
    async removeNote(id) {
        this.notes = this.notes.filter(n => n.id !== id);
        this.saveNotes();
        
        if (currentUser && firebaseDb) {
            try {
                await firebaseDb.collection('users').doc(currentUser.uid)
                    .collection('notes').doc(id).delete();
            } catch (error) {
                console.error('Error removing note:', error);
            }
        }
    },
    
    saveNotes() {
        localStorage.setItem('chronos_notes', JSON.stringify(this.notes));
    },
    
    loadNotes() {
        const stored = localStorage.getItem('chronos_notes');
        if (stored) {
            this.notes = JSON.parse(stored);
        }
    },
    
    getNotesForItem(slug) {
        return this.notes.filter(n => n.itemSlug === slug);
    },
    
    getItemsByCollection(collection) {
        return this.library.filter(i => i.collection === collection);
    }
};

// ==================== AUTH FUNCTIONS ====================
async function signInWithGoogle() {
    if (!firebaseAuth) {
        showToast('Firebase not configured. Please set up Firebase first.', 'error');
        return;
    }
    
    const provider = new firebase.auth.GoogleAuthProvider();
    try {
        showLoading('Signing in...');
        const result = await firebaseAuth.signInWithPopup(provider);
        const user = result.user;
        
        // Save user data to Firestore
        if (firebaseDb) {
            await firebaseDb.collection('users').doc(user.uid).set({
                uid: user.uid,
                email: user.email,
                displayName: user.displayName,
                photoURL: user.photoURL,
                createdAt: firebase.firestore.FieldValue.serverTimestamp(),
                lastLogin: firebase.firestore.FieldValue.serverTimestamp()
            }, { merge: true });
        }
        
        showToast(`Welcome, ${user.displayName}!`, 'success');
        closeAuthModal();
        hideLoading();
    } catch (error) {
        hideLoading();
        showToast('Sign in failed: ' + error.message, 'error');
        console.error('Sign in error:', error);
    }
}

async function signInAsGuest() {
    if (!firebaseAuth) {
        showToast('Firebase not configured. Please set up Firebase first.', 'error');
        return;
    }
    
    try {
        showLoading('Continuing as guest...');
        const result = await firebaseAuth.signInAnonymously();
        const user = result.user;
        
        // Save guest user data to Firestore
        if (firebaseDb) {
            await firebaseDb.collection('users').doc(user.uid).set({
                uid: user.uid,
                email: null,
                displayName: 'Guest',
                photoURL: null,
                isAnonymous: true,
                createdAt: firebase.firestore.FieldValue.serverTimestamp(),
                lastLogin: firebase.firestore.FieldValue.serverTimestamp()
            }, { merge: true });
        }
        
        showToast('Welcome, Guest!', 'success');
        closeAuthModal();
        hideLoading();
    } catch (error) {
        hideLoading();
        showToast('Guest sign in failed: ' + error.message, 'error');
        console.error('Guest sign in error:', error);
    }
}

async function signOut() {
    if (!firebaseAuth) return;
    
    try {
        await firebaseAuth.signOut();
        showToast('Signed out successfully', 'success');
    } catch (error) {
        showToast('Sign out failed: ' + error.message, 'error');
    }
}

function updateUIForAuthState() {
    const navUser = document.getElementById('navUser');
    const mobileUser = document.getElementById('mobileUser');
    
    if (currentUser) {
        const displayName = currentUser.displayName || currentUser.email?.split('@')[0] || 'Guest';
        const photoURL = currentUser.photoURL || `https://ui-avatars.com/api/?name=${encodeURIComponent(displayName)}&background=d4af37&color=0a0a0f`;
        
        navUser.innerHTML = `
            <div class="user-profile">
                <img src="${photoURL}" alt="${displayName}" class="user-avatar">
                <span class="user-name">${displayName}</span>
                <div class="user-dropdown">
                    <div class="dropdown-item" onclick="Router.navigate('library')">
                        <i class="fas fa-bookmark"></i> My Library
                    </div>
                    <div class="dropdown-item" onclick="signOut()">
                        <i class="fas fa-sign-out-alt"></i> Sign Out
                    </div>
                </div>
            </div>
        `;
        
        if (mobileUser) {
            mobileUser.innerHTML = `
                <div class="mobile-user-info" style="padding: 1rem; text-align: center;">
                    <img src="${photoURL}" alt="${displayName}" style="width: 60px; height: 60px; border-radius: 50%; margin-bottom: 0.5rem; border: 2px solid var(--accent-gold);">
                    <p style="color: var(--text-primary); font-weight: 600;">${displayName}</p>
                </div>
                <a href="#/library" class="mobile-link">My Library</a>
                <a href="#" class="mobile-link" onclick="signOut()">Sign Out</a>
            `;
        }
        
        // Update greeting if on home page
        const greeting = document.getElementById('userGreeting');
        if (greeting) {
            greeting.textContent = `Hi, ${displayName.split(' ')[0]}`;
        }
    } else {
        navUser.innerHTML = `
            <button class="login-btn" id="loginBtn" onclick="openAuthModal()">
                <i class="fab fa-google"></i> Sign In
            </button>
        `;
        
        if (mobileUser) {
            mobileUser.innerHTML = `
                <button class="login-btn" onclick="openAuthModal()" style="width: 100%; margin-top: 1rem;">
                    <i class="fab fa-google"></i> Sign In
                </button>
            `;
        }
    }
}

async function loadUserLibrary() {
    if (!currentUser || !firebaseDb) return;
    
    try {
        const snapshot = await firebaseDb.collection('users')
            .doc(currentUser.uid)
            .collection('bookmarks')
            .orderBy('bookmarkedAt', 'desc')
            .get();
        
        const cloudLibrary = snapshot.docs.map(doc => ({
            slug: doc.id,
            ...doc.data()
        }));
        
        // Merge with local library
        const localSlugs = new Set(State.library.map(i => i.slug));
        cloudLibrary.forEach(item => {
            if (!localSlugs.has(item.slug)) {
                State.library.push(item);
            }
        });
        
        State.saveLibrary();
    } catch (error) {
        console.error('Error loading library:', error);
    }
}

// ==================== ROUTER ====================
const Router = {
    currentRoute: '',
    initialized: false,
    
    init() {
        if (this.initialized) return;
        this.initialized = true;
        
        window.addEventListener('hashchange', () => this.handleRoute());
        
        document.addEventListener('click', (e) => {
            const link = e.target.closest('[data-route]');
            if (link) {
                e.preventDefault();
                const route = link.dataset.route;
                this.navigate(route);
            }
        });
        
        // Handle initial route
        this.handleRoute();
    },
    
    navigate(route, params = {}) {
        let hash = '#/' + route;
        if (params.slug) {
            hash += '/' + params.slug;
        }
        window.location.hash = hash;
    },
    
    handleRoute() {
        try {
            const hash = window.location.hash || '#/';
        const parts = hash.replace('#/', '').split('/').filter(Boolean);
        const route = parts[0] || 'home';
        const slug = parts[1];
        
        this.currentRoute = route;
        
        // Update nav active states
        document.querySelectorAll('.nav-link, .mobile-link').forEach(link => {
            link.classList.toggle('active', link.dataset.route === route);
        });
        
        // Close mobile menu
        document.getElementById('mobileMenu')?.classList.remove('active');
        
        const app = document.getElementById('app');
        
        // Animate page transition
        gsap.to(app, {
            opacity: 0,
            y: 10,
            duration: 0.2,
            onComplete: () => {
                switch(route) {
                    case 'home':
                        app.innerHTML = renderHomePage();
                        initHomePage();
                        break;
                    case 'history':
                        if (slug) {
                            renderHistoryPage(slug);
                        } else {
                            this.navigate('home');
                        }
                        break;
                    case 'explore':
                        app.innerHTML = renderExplorePage();
                        initExplorePage();
                        break;
                    case 'map':
                        app.innerHTML = renderMapPage();
                        initMapPage();
                        break;
                    case 'quotes':
                        app.innerHTML = renderQuotesPage();
                        break;
                    case 'library':
                        app.innerHTML = renderLibraryPage();
                        break;
                    case 'timeline-generator':
                        app.innerHTML = renderTimelineGeneratorPage();
                        initTimelineGeneratorPage();
                        break;
                    case 'future-prediction':
                        app.innerHTML = renderFuturePredictionPage();
                        initFuturePredictionPage();
                        break;
                    case 'compare-legends':
                        app.innerHTML = renderCompareLegendsPage();
                        initCompareLegendsPage();
                        break;
                    default:
                        this.navigate('home');
                }
                
                // Animate in
                gsap.fromTo(app, 
                    { opacity: 0, y: 20 },
                    { opacity: 1, y: 0, duration: 0.4, ease: 'power2.out' }
                );
                
                window.scrollTo({ top: 0, behavior: 'smooth' });
            }
        });
        } catch (error) {
            console.error('Route handling error:', error);
            // Fallback to home page on error
            const app = document.getElementById('app');
            if (app) {
                app.innerHTML = renderHomePage();
                initHomePage();
            }
        }
    }
};

// ==================== WIKIPEDIA API ====================
const WikipediaAPI = {
    async search(query) {
        try {
            const response = await fetch(
                `${CONFIG.WIKI_API}?action=query&list=search&srsearch=${encodeURIComponent(query)}&format=json&origin=*&srlimit=8`
            );
            const data = await response.json();
            return data.query.search;
        } catch (error) {
            console.error('Search error:', error);
            return [];
        }
    },
    
    async getPage(title) {
        try {
            const searchResponse = await fetch(
                `${CONFIG.WIKI_API}?action=query&list=search&srsearch=${encodeURIComponent(title)}&format=json&origin=*&srlimit=1`
            );
            const searchData = await searchResponse.json();
            
            if (!searchData.query.search.length) return null;
            
            const exactTitle = searchData.query.search[0].title;
            
            const contentResponse = await fetch(
                `${CONFIG.WIKI_API}?action=query&prop=extracts|pageimages&exintro=false&explaintext=false&exsentences=30&piprop=original|thumbnail&pithumbsize=800&titles=${encodeURIComponent(exactTitle)}&format=json&origin=*`
            );
            const contentData = await contentResponse.json();
            const pages = contentData.query.pages;
            const pageId = Object.keys(pages)[0];
            const page = pages[pageId];
            
            if (pageId === '-1' || !page.extract) return null;
            
            let imageUrl = page.thumbnail?.source || page.original?.source || CONFIG.DEFAULT_IMAGE;
            
            const catResponse = await fetch(
                `${CONFIG.WIKI_API}?action=query&prop=categories&titles=${encodeURIComponent(exactTitle)}&format=json&origin=*&cllimit=10`
            );
            const catData = await catResponse.json();
            const catPages = catData.query.pages;
            const categories = catPages[Object.keys(catPages)[0]].categories || [];
            
            const yearMatch = exactTitle.match(/(\d{3,4})/);
            const year = yearMatch ? yearMatch[1] : this.extractYear(categories);
            
            const timeline = this.generateTimeline(page.extract);
            const facts = this.generateFacts(page.extract, categories);
            
            return {
                title: page.title,
                extract: this.formatExtract(page.extract),
                image: imageUrl,
                year: year,
                categories: categories.map(c => c.title.replace('Category:', '')),
                timeline: timeline,
                facts: facts,
                slug: this.slugify(page.title)
            };
        } catch (error) {
            console.error('Get page error:', error);
            return null;
        }
    },
    
    extractYear(categories) {
        for (const cat of categories) {
            const match = cat.title.match(/(\d{3,4})/);
            if (match) return match[1];
        }
        return 'Historical Period';
    },
    
    formatExtract(extract) {
        if (!extract) return '<p>No information available.</p>';
        
        return extract
            .replace(/\[\d+\]/g, '')
            .replace(/\{\{[^}]+\}\}/g, '')
            .replace(/\[\[([^|\]]+)\|([^\]]+)\]\]/g, '$2')
            .replace(/\[\[([^\]]+)\]\]/g, '$1')
            .replace(/'''([^']+)'''/g, '<strong>$1</strong>')
            .replace(/''([^']+)''/g, '<em>$1</em>')
            .split(/\n+/)
            .filter(p => p.trim().length > 30)
            .slice(0, 5)
            .map(p => `<p>${p.trim()}</p>`)
            .join('');
    },
    
    generateTimeline(extract) {
        const events = [];
        const sentences = extract?.split(/[.!?]+/) || [];
        
        sentences.forEach(sentence => {
            const yearMatch = sentence.match(/\b(1\d{3}|20\d{2})\b/);
            if (yearMatch && sentence.trim().length > 40) {
                events.push({
                    year: yearMatch[1],
                    title: sentence.trim().substring(0, 60) + '...'
                });
            }
        });
        
        return events.slice(0, 5);
    },
    
    generateFacts(extract, categories) {
        const facts = [];
        
        const relevantCats = categories.filter(c => 
            c.title.includes('born') || 
            c.title.includes('died') ||
            c.title.includes('century') ||
            c.title.includes('Empire') ||
            c.title.includes('War')
        );
        
        if (relevantCats.length > 0) {
            facts.push({
                label: 'Category',
                value: relevantCats[0].title.replace('Category:', '').substring(0, 30)
            });
        }
        
        facts.push(
            { label: 'Source', value: 'Wikipedia' },
            { label: 'Type', value: 'Historical Topic' }
        );
        
        return facts;
    },
    
    slugify(text) {
        return text.toLowerCase()
            .replace(/[^\w\s-]/g, '')
            .replace(/\s+/g, '-')
            .substring(0, 50);
    }
};

// ==================== RENDER FUNCTIONS ====================
function renderHomePage() {
    const dailyEvents = getDailyEvents();
    const displayName = currentUser?.displayName?.split(' ')[0] || currentUser?.email?.split('@')[0] || null;
    
    return `
        <div class="home-page">
            <section class="hero-section">
                ${displayName ? `<p class="greeting" id="userGreeting">Hi, ${displayName}</p>` : ''}
                <h1 class="hero-title">Journey Through Time</h1>
                <p class="hero-subtitle">Discover history with AI-powered search and personalized timelines</p>
                
                <div class="search-container">
                    <div class="search-box">
                        <i class="fas fa-search"></i>
                        <input type="text" class="search-input" id="searchInput" 
                            placeholder="Search any historical topic... (e.g., Napoleon, WW2, Roman Empire)"
                            autocomplete="off">
                        <button class="search-btn" id="searchBtn">Search</button>
                    </div>
                    <div class="search-suggestions" id="searchSuggestions"></div>
                </div>
            </section>
            
            <section class="daily-history-section">
                <div class="section-header">
                    <h2 class="section-title"><i class="fas fa-calendar-day"></i> On This Day in History</h2>
                    <span class="date-badge"><i class="fas fa-clock"></i> ${new Date().toLocaleDateString('en-US', { month: 'long', day: 'numeric' })}</span>
                </div>
                <div class="daily-cards-scroll">
                    ${dailyEvents.map(event => `
                        <div class="daily-card" data-slug="${event.slug}">
                            <div class="daily-card-image" style="background-image: url('${event.image}')">
                                <span class="daily-card-year">${event.year}</span>
                            </div>
                            <div class="daily-card-content">
                                <h3 class="daily-card-title">${event.title}</h3>
                                <p class="daily-card-desc">${event.desc}</p>
                                <button class="daily-card-btn">
                                    Explore Full Story <i class="fas fa-arrow-right"></i>
                                </button>
                            </div>
                        </div>
                    `).join('')}
                </div>
            </section>
            
            <section class="timeline-cta-section">
                <i class="fas fa-wand-magic-sparkles timeline-cta-icon"></i>
                <h2 class="timeline-cta-title">Create Your Personal Timeline</h2>
                <p class="timeline-cta-desc">Discover the major historical events that happened during your lifetime, tailored to your interests.</p>
                <button class="timeline-cta-btn" onclick="Router.navigate('timeline-generator')">
                    <i class="fas fa-sparkles"></i> Generate My Timeline
                </button>
            </section>
            
            <section class="featured-section">
                <div class="section-header">
                    <h2 class="section-title"><i class="fas fa-fire"></i> Featured Topics</h2>
                </div>
                <div class="topics-grid">
                    ${CONFIG.FEATURED_TOPICS.map((topic, index) => `
                        <div class="topic-card" data-slug="${topic.id}" style="animation-delay: ${index * 0.1}s">
                            <div class="topic-image" style="background-image: url('${topic.image}')"></div>
                            <div class="topic-content">
                                <p class="topic-era">${topic.era}</p>
                                <h3 class="topic-name">${topic.title}</h3>
                                <p class="topic-desc">${topic.desc}</p>
                            </div>
                        </div>
                    `).join('')}
                </div>
            </section>
            
            <section class="timeline-section-home">
                <div class="timeline-header">
                    <h2><i class="fas fa-history"></i> Travel Through Time</h2>
                    <p>Drag the slider to explore different eras</p>
                </div>
                <div class="timeline-container">
                    <div class="timeline-labels">
                        <span class="timeline-start">500 BC</span>
                        <span class="timeline-current" id="currentYear">1000 AD</span>
                        <span class="timeline-end">2000 AD</span>
                    </div>
                    <div class="slider-wrapper">
                        <div class="slider-track"></div>
                        <input type="range" class="timeline-slider" id="timelineSlider" min="-500" max="2000" value="1000">
                        <div class="slider-fill" id="sliderFill"></div>
                    </div>
                    <div class="timeline-hint">Drag to travel through time</div>
                    <div class="timeline-era" id="timelineEra">High Medieval Period</div>
                    <button class="explore-era-btn visible" id="exploreEraBtn">Explore This Era</button>
                </div>
            </section>
        </div>
    `;
}

function initHomePage() {
    // Search functionality
    const searchInput = document.getElementById('searchInput');
    const searchBtn = document.getElementById('searchBtn');
    const suggestions = document.getElementById('searchSuggestions');
    let debounceTimer;
    
    searchInput?.addEventListener('input', (e) => {
        clearTimeout(debounceTimer);
        const query = e.target.value.trim();
        
        if (query.length < 2) {
            suggestions.classList.remove('active');
            return;
        }
        
        debounceTimer = setTimeout(async () => {
            const results = await WikipediaAPI.search(query);
            showSuggestions(results, query);
        }, 300);
    });
    
    searchBtn?.addEventListener('click', () => {
        const query = searchInput.value.trim();
        if (query) {
            Router.navigate('history', { slug: WikipediaAPI.slugify(query) });
        }
    });
    
    searchInput?.addEventListener('keypress', (e) => {
        if (e.key === 'Enter') {
            searchBtn.click();
        }
    });
    
    document.addEventListener('click', (e) => {
        if (!e.target.closest('.search-container')) {
            suggestions?.classList.remove('active');
        }
    });
    
    // Topic card clicks
    document.querySelectorAll('.topic-card, .daily-card').forEach(card => {
        card.addEventListener('click', (e) => {
            if (e.target.closest('.daily-card-btn')) {
                const slug = card.dataset.slug;
                Router.navigate('history', { slug });
            } else if (!e.target.closest('button')) {
                const slug = card.dataset.slug;
                Router.navigate('history', { slug });
            }
        });
    });
    
    // Timeline slider
    initTimelineSlider();
    
    // Animate elements - daily cards are visible immediately, no scroll animation
    gsap.from('.daily-card', {
        opacity: 0,
        y: 20,
        stagger: 0.1,
        duration: 0.4,
        ease: 'power2.out'
    });
    
    // Topic cards - visible immediately with subtle animation
    gsap.from('.topic-card', {
        opacity: 0,
        y: 20,
        stagger: 0.08,
        duration: 0.4,
        ease: 'power2.out',
        delay: 0.2
    });
}

function initTimelineSlider() {
    const slider = document.getElementById('timelineSlider');
    const currentYear = document.getElementById('currentYear');
    const timelineEra = document.getElementById('timelineEra');
    const sliderFill = document.getElementById('sliderFill');
    const exploreBtn = document.getElementById('exploreEraBtn');
    
    if (!slider) return;
    
    let currentEra = 'medieval';
    
    function updateSlider(value) {
        const year = parseInt(value);
        const displayYear = year < 0 ? `${Math.abs(year)} BC` : `${year} AD`;
        
        currentYear.textContent = displayYear;
        
        const min = parseInt(slider.min);
        const max = parseInt(slider.max);
        const percentage = ((year - min) / (max - min)) * 100;
        sliderFill.style.width = `${percentage}%`;
        
        let eraName, eraKey;
        
        if (year < 0) {
            eraName = 'Ancient Period';
            eraKey = 'ancient';
        } else if (year < 500) {
            eraName = 'Classical Antiquity';
            eraKey = 'ancient';
        } else if (year < 1000) {
            eraName = 'Early Medieval Period';
            eraKey = 'medieval';
        } else if (year < 1400) {
            eraName = 'High Medieval Period';
            eraKey = 'medieval';
        } else if (year < 1600) {
            eraName = 'Renaissance Era';
            eraKey = 'renaissance';
        } else if (year < 1800) {
            eraName = 'Age of Enlightenment';
            eraKey = 'renaissance';
        } else if (year < 1900) {
            eraName = 'Industrial Revolution';
            eraKey = 'industrial';
        } else {
            eraName = 'Modern Era';
            eraKey = 'modern';
        }
        
        timelineEra.textContent = eraName;
        currentEra = eraKey;
    }
    
    slider.addEventListener('input', (e) => {
        updateSlider(e.target.value);
    });
    
    exploreBtn?.addEventListener('click', () => {
        const topics = CONFIG.ERA_TOPICS[currentEra] || CONFIG.ERA_TOPICS.medieval;
        const randomTopic = topics[Math.floor(Math.random() * topics.length)];
        Router.navigate('history', { slug: WikipediaAPI.slugify(randomTopic) });
    });
    
    updateSlider(1000);
}

function showSuggestions(results, query) {
    const suggestions = document.getElementById('searchSuggestions');
    
    const featuredMatches = CONFIG.FEATURED_TOPICS.filter(t => 
        t.title.toLowerCase().includes(query.toLowerCase())
    );
    
    let html = '';
    
    if (featuredMatches.length) {
        html += `<div class="suggestion-category">Featured</div>`;
        featuredMatches.forEach(topic => {
            html += `
                <div class="suggestion-item" data-slug="${topic.id}">
                    <div class="suggestion-title">⭐ ${topic.title}</div>
                    <div class="suggestion-desc">${topic.era} — ${topic.desc}</div>
                </div>
            `;
        });
    }
    
    if (results.length) {
        html += `<div class="suggestion-category">From Wikipedia</div>`;
        results.slice(0, 5).forEach(result => {
            html += `
                <div class="suggestion-item" data-title="${result.title}">
                    <div class="suggestion-title">${result.title}</div>
                    <div class="suggestion-desc">${result.snippet.replace(/<[^>]*>/g, '').substring(0, 80)}...</div>
                </div>
            `;
        });
    }
    
    suggestions.innerHTML = html;
    suggestions.classList.add('active');
    
    suggestions.querySelectorAll('.suggestion-item').forEach(item => {
        item.addEventListener('click', () => {
            const slug = item.dataset.slug || WikipediaAPI.slugify(item.dataset.title);
            Router.navigate('history', { slug });
        });
    });
}

// ==================== DAILY EVENTS ====================
function getDailyEvents() {
    const today = new Date();
    const month = String(today.getMonth() + 1).padStart(2, '0');
    const day = String(today.getDate()).padStart(2, '0');
    const dateKey = `${month}-${day}`;
    
    // Always return events - either from today's date or fallback to defaults
    let events = CONFIG.DAILY_EVENTS[dateKey];
    if (!events || events.length === 0) {
        events = CONFIG.DEFAULT_EVENTS;
    }
    return events.slice(0, 4);
}

// ==================== HISTORY PAGE ====================
async function renderHistoryPage(slug) {
    const app = document.getElementById('app');
    showLoading('Loading historical data...');
    
    const featured = CONFIG.FEATURED_TOPICS.find(t => t.id === slug);
    let data;
    
    if (featured) {
        const wikiData = await WikipediaAPI.getPage(featured.title);
        data = wikiData || {
            title: featured.title,
            extract: `<p>${featured.desc}</p>`,
            image: featured.image.replace('w=400', 'w=1920').replace('h=300', 'h=1080'),
            year: featured.era,
            slug: featured.id,
            timeline: [],
            facts: [
                { label: 'Era', value: featured.era },
                { label: 'Type', value: 'Historical Topic' }
            ],
            categories: []
        };
    } else {
        data = await WikipediaAPI.getPage(slug.replace(/-/g, ' '));
    }
    
    hideLoading();
    
    if (!data) {
        showToast('Topic not found. Try another search.', 'error');
        Router.navigate('home');
        return;
    }
    
    const isSaved = State.isInLibrary(data.slug);
    const suggestions = getSuggestions(data.title);
    
    app.innerHTML = `
        <div class="history-page">
            <section class="history-hero" style="background-image: url('${data.image}')">
                <div class="history-hero-content">
                    <div class="history-meta">
                        <span class="history-era">${data.year}</span>
                        ${data.categories[0] ? `<span class="history-category">${data.categories[0]}</span>` : ''}
                    </div>
                    <h1 class="history-title">${data.title}</h1>
                    <div class="history-actions">
                        <button class="action-btn ${isSaved ? 'saved' : ''}" id="saveBtn">
                            <i class="fas ${isSaved ? 'fa-check' : 'fa-bookmark'}"></i>
                            <span>${isSaved ? 'Saved' : 'Save'}</span>
                        </button>
                        <button class="action-btn" id="listenBtn">
                            <i class="fas fa-headphones"></i>
                            <span>Listen</span>
                        </button>
                        <button class="action-btn share-btn" id="shareBtn">
                            <i class="fas fa-share-alt"></i>
                            <span>Share</span>
                        </button>
                    </div>
                </div>
            </section>
            
            <div class="history-content">
                <div class="history-main">
                    <div class="history-text">
                        ${data.extract}
                    </div>
                    
                    ${data.timeline.length ? `
                        <section class="timeline-section">
                            <h2>Timeline</h2>
                            <div class="timeline">
                                ${data.timeline.map(event => `
                                    <div class="timeline-item">
                                        <div class="timeline-year">${event.year}</div>
                                        <div class="timeline-title">${event.title}</div>
                                    </div>
                                `).join('')}
                            </div>
                        </section>
                    ` : ''}
                    
                    <section class="summary-section">
                        <h3 class="summary-title">Key Highlights</h3>
                        <ul class="summary-list">
                            ${generateSummaryPoints(data.extract).map(p => `<li>${p}</li>`).join('')}
                        </ul>
                    </section>
                    
                    <section class="suggestions-section">
                        <h3 class="suggestions-title">If you liked this, <span>explore:</span></h3>
                        <div class="suggestions-grid">
                            ${suggestions.map(s => `
                                <div class="suggestion-card" data-slug="${WikipediaAPI.slugify(s)}">
                                    <div class="suggestion-card-title">${s}</div>
                                    <div class="suggestion-card-desc">Related topic</div>
                                </div>
                            `).join('')}
                        </div>
                    </section>
                </div>
                
                <aside class="history-sidebar">
                    <h2>Key Facts</h2>
                    <div class="facts-grid">
                        ${data.facts.map(fact => `
                            <div class="fact-card">
                                <div class="fact-label">${fact.label}</div>
                                <div class="fact-value">${fact.value}</div>
                            </div>
                        `).join('')}
                    </div>
                    
                    <div class="wiki-attribution" style="margin-top: 2rem; padding: 1rem; background: rgba(212, 175, 55, 0.05); border-radius: 12px;">
                        <p style="font-size: 0.85rem; color: var(--text-muted); text-align: center;">
                            <i class="fas fa-book" style="color: var(--accent-gold);"></i><br>
                            Content from <a href="https://en.wikipedia.org/wiki/${encodeURIComponent(data.title)}" target="_blank" style="color: var(--accent-gold);">Wikipedia</a>
                        </p>
                    </div>
                </aside>
            </div>
        </div>
    `;
    
    // Save button
    document.getElementById('saveBtn')?.addEventListener('click', async function() {
        const item = {
            slug: data.slug,
            title: data.title,
            era: data.year,
            image: data.image,
            desc: data.extract.replace(/<[^>]*>/g, '').substring(0, 100) + '...'
        };
        
        if (await State.addToLibrary(item)) {
            this.classList.add('saved');
            this.innerHTML = '<i class="fas fa-check"></i><span>Saved</span>';
            showToast('Added to your library!', 'success');
        } else {
            showToast('Already in your library', 'info');
        }
    });
    
    // Listen button
    document.getElementById('listenBtn')?.addEventListener('click', () => {
        const text = data.extract.replace(/<[^>]*>/g, '');
        playAudio(text, data.title);
    });
    
    // Share button
    document.getElementById('shareBtn')?.addEventListener('click', () => {
        openShareModal(data);
    });
    
    // Suggestion cards
    document.querySelectorAll('.suggestion-card').forEach(card => {
        card.addEventListener('click', () => {
            Router.navigate('history', { slug: card.dataset.slug });
        });
    });
}

function generateSummaryPoints(extract) {
    const text = extract.replace(/<[^>]*>/g, '');
    const sentences = text.split(/[.!?]+/).filter(s => s.trim().length > 30 && s.trim().length < 120);
    return sentences.slice(0, 5).map(s => s.trim() + '.');
}

function getSuggestions(title) {
    const lowerTitle = title.toLowerCase();
    for (const key in CONFIG.SUGGESTIONS) {
        if (lowerTitle.includes(key)) {
            return CONFIG.SUGGESTIONS[key];
        }
    }
    return CONFIG.SUGGESTIONS.default;
}

// ==================== EXPLORE PAGE ====================
function renderExplorePage() {
    return `
        <div class="home-page">
            <section class="hero-section">
                <h1 class="hero-title">Explore History</h1>
                <p class="hero-subtitle">Discover topics from around the world</p>
            </section>
            
            <section class="featured-section">
                <div class="section-header">
                    <h2 class="section-title"><i class="fas fa-globe"></i> All Topics</h2>
                </div>
                <div class="topics-grid">
                    ${CONFIG.FEATURED_TOPICS.map(topic => `
                        <div class="topic-card" data-slug="${topic.id}">
                            <div class="topic-image" style="background-image: url('${topic.image}')"></div>
                            <div class="topic-content">
                                <p class="topic-era">${topic.era}</p>
                                <h3 class="topic-name">${topic.title}</h3>
                                <p class="topic-desc">${topic.desc}</p>
                            </div>
                        </div>
                    `).join('')}
                </div>
            </section>
        </div>
    `;
}

function initExplorePage() {
    document.querySelectorAll('.topic-card').forEach(card => {
        card.addEventListener('click', () => {
            Router.navigate('history', { slug: card.dataset.slug });
        });
    });
}

// ==================== MAP PAGE ====================
function renderMapPage() {
    return `
        <div class="map-page">
            <div class="map-header">
                <h1 class="map-title">Interactive World Map</h1>
                <p class="map-subtitle">Click on any country to explore its history</p>
            </div>
            
            <div class="map-container">
                <svg class="world-map" viewBox="0 0 1000 500" xmlns="http://www.w3.org/2000/svg">
                    <!-- North America - Americas (Blue) -->
                    <path class="map-country americas" data-country="US" data-name="United States" 
                        d="M150,120 L280,110 L300,180 L260,220 L180,200 L140,160 Z" />
                    <path class="map-country americas" data-country="CA" data-name="Canada" 
                        d="M140,50 L320,40 L340,100 L280,110 L150,120 L120,80 Z" />
                    <path class="map-country americas" data-country="MX" data-name="Mexico" 
                        d="M180,200 L260,220 L250,280 L200,300 L170,250 Z" />
                    <!-- South America - Americas (Blue) -->
                    <path class="map-country americas" data-country="BR" data-name="Brazil" 
                        d="M280,300 L380,290 L400,380 L350,420 L300,400 L270,350 Z" />
                    <path class="map-country americas" data-country="AR" data-name="Argentina" 
                        d="M270,400 L310,410 L300,480 L280,470 Z" />
                    <!-- Europe - Europe (Gold/Brown) -->
                    <path class="map-country europe" data-country="GB" data-name="United Kingdom" 
                        d="M460,100 L490,95 L495,130 L470,135 L455,120 Z" />
                    <path class="map-country europe" data-country="FR" data-name="France" 
                        d="M470,140 L510,135 L515,170 L480,175 L465,160 Z" />
                    <path class="map-country europe" data-country="DE" data-name="Germany" 
                        d="M510,125 L550,120 L555,155 L520,160 L508,145 Z" />
                    <path class="map-country europe" data-country="IT" data-name="Italy" 
                        d="M520,165 L540,160 L545,200 L530,210 L515,185 Z" />
                    <!-- Russia - Asia (Purple) -->
                    <path class="map-country asia" data-country="RU" data-name="Russia" 
                        d="M560,60 L850,50 L880,150 L700,160 L580,140 L550,100 Z" />
                    <!-- Africa - Africa (Green) -->
                    <path class="map-country africa" data-country="EG" data-name="Egypt" 
                        d="M530,220 L580,215 L585,250 L540,255 L525,240 Z" />
                    <path class="map-country africa" data-country="ZA" data-name="South Africa" 
                        d="M520,380 L580,375 L590,420 L540,430 L510,410 Z" />
                    <!-- Asia - Asia (Purple) -->
                    <path class="map-country asia" data-country="CN" data-name="China" 
                        d="M680,160 L820,150 L850,220 L780,250 L700,240 L670,200 Z" />
                    <path class="map-country asia" data-country="IN" data-name="India" 
                        d="M640,220 L690,215 L700,280 L660,300 L630,260 Z" />
                    <path class="map-country asia" data-country="JP" data-name="Japan" 
                        d="M860,170 L890,165 L895,210 L870,220 L855,200 Z" />
                    <!-- Oceania - Oceania (Pink) -->
                    <path class="map-country oceania" data-country="AU" data-name="Australia" 
                        d="M780,350 L920,340 L940,430 L850,450 L770,420 Z" />
                </svg>
                <div class="map-tooltip" id="mapTooltip"></div>
            </div>
            
            <div class="map-legend">
                <div class="legend-item">
                    <div class="legend-color europe"></div>
                    <span>Europe</span>
                </div>
                <div class="legend-item">
                    <div class="legend-color asia"></div>
                    <span>Asia</span>
                </div>
                <div class="legend-item">
                    <div class="legend-color africa"></div>
                    <span>Africa</span>
                </div>
                <div class="legend-item">
                    <div class="legend-color americas"></div>
                    <span>Americas</span>
                </div>
                <div class="legend-item">
                    <div class="legend-color oceania"></div>
                    <span>Oceania</span>
                </div>
            </div>
        </div>
    `;
}

function initMapPage() {
    const tooltip = document.getElementById('mapTooltip');
    
    document.querySelectorAll('.map-country').forEach(country => {
        country.addEventListener('mouseenter', (e) => {
            const countryName = country.dataset.name;
            tooltip.textContent = countryName;
            tooltip.classList.add('visible');
        });
        
        country.addEventListener('mousemove', (e) => {
            const rect = country.closest('.map-container').getBoundingClientRect();
            tooltip.style.left = (e.clientX - rect.left + 10) + 'px';
            tooltip.style.top = (e.clientY - rect.top - 30) + 'px';
        });
        
        country.addEventListener('mouseleave', () => {
            tooltip.classList.remove('visible');
        });
        
        country.addEventListener('click', () => {
            const countryCode = country.dataset.country;
            const topics = CONFIG.COUNTRY_TOPICS[countryCode];
            
            if (topics && topics.length > 0) {
                const randomTopic = topics[Math.floor(Math.random() * topics.length)];
                Router.navigate('history', { slug: WikipediaAPI.slugify(randomTopic) });
            } else {
                showToast('History coming soon for this region!', 'error');
            }
        });
    });
}

// ==================== QUOTES PAGE ====================
function renderQuotesPage() {
    return `
        <div class="quotes-page">
            <div class="quotes-header">
                <h1 class="quotes-title">Words of Wisdom</h1>
                <p style="color: var(--text-secondary);">Timeless quotes from history</p>
            </div>
            
            <div class="quotes-grid">
                ${CONFIG.QUOTES.map((quote, index) => `
                    <div class="quote-card" style="animation-delay: ${index * 0.1}s">
                        <i class="fas fa-quote-left quote-icon"></i>
                        <p class="quote-text">"${quote.text}"</p>
                        <p class="quote-author">— ${quote.author}</p>
                        <div class="quote-actions">
                            <button class="quote-btn" onclick="copyQuote('${quote.text}', '${quote.author}')">
                                <i class="fas fa-copy"></i> Copy
                            </button>
                            <button class="quote-btn" onclick="shareQuote('${quote.text}', '${quote.author}')">
                                <i class="fas fa-share"></i> Share
                            </button>
                        </div>
                    </div>
                `).join('')}
            </div>
        </div>
    `;
}

function copyQuote(text, author) {
    const fullText = `"${text}" — ${author}`;
    navigator.clipboard.writeText(fullText).then(() => {
        showToast('Quote copied to clipboard!', 'success');
    });
}

function shareQuote(text, author) {
    const fullText = `"${text}" — ${author}`;
    if (navigator.share) {
        navigator.share({
            title: 'History Quote from Chronos',
            text: fullText
        });
    } else {
        navigator.clipboard.writeText(fullText).then(() => {
            showToast('Quote copied to clipboard!', 'success');
        });
    }
}

// ==================== LIBRARY PAGE ====================
function renderLibraryPage() {
    return renderEnhancedLibraryPage();
}

// ==================== TIMELINE GENERATOR PAGE ====================
function renderTimelineGeneratorPage() {
    return `
        <div class="timeline-generator-page">
            <div class="timeline-generator-hero">
                <h1><i class="fas fa-wand-magic-sparkles"></i> Your Personal Timeline</h1>
                <p>Discover the major historical events that shaped your lifetime</p>
            </div>
            
            <div class="timeline-form-container">
                <form class="timeline-form" id="timelineForm">
                    <div class="form-group">
                        <label for="birthYear">When were you born?</label>
                        <input type="number" id="birthYear" min="1900" max="2025" placeholder="e.g., 1990" required>
                    </div>
                    
                    <div class="form-group">
                        <label>What interests you? (Select all that apply)</label>
                        <div class="interest-tags" id="interestTags">
                            <button type="button" class="interest-tag" data-value="war">
                                <i class="fas fa-shield-alt"></i> Wars & Battles
                            </button>
                            <button type="button" class="interest-tag" data-value="tech">
                                <i class="fas fa-microchip"></i> Technology
                            </button>
                            <button type="button" class="interest-tag" data-value="empires">
                                <i class="fas fa-crown"></i> Empires & Kings
                            </button>
                            <button type="button" class="interest-tag" data-value="inventions">
                                <i class="fas fa-lightbulb"></i> Inventions
                            </button>
                            <button type="button" class="interest-tag" data-value="space">
                                <i class="fas fa-rocket"></i> Space Exploration
                            </button>
                            <button type="button" class="interest-tag" data-value="art">
                                <i class="fas fa-palette"></i> Art & Culture
                            </button>
                            <button type="button" class="interest-tag" data-value="science">
                                <i class="fas fa-flask"></i> Science
                            </button>
                            <button type="button" class="interest-tag" data-value="sports">
                                <i class="fas fa-trophy"></i> Sports
                            </button>
                        </div>
                    </div>
                    
                    <button type="submit" class="generate-timeline-btn">
                        <i class="fas fa-sparkles"></i> Generate My Timeline
                    </button>
                </form>
            </div>
            
            <div class="generated-timeline" id="generatedTimeline" style="display: none;"></div>
        </div>
    `;
}

function initTimelineGeneratorPage() {
    const form = document.getElementById('timelineForm');
    const interestTags = document.querySelectorAll('.interest-tag');
    
    interestTags.forEach(tag => {
        tag.addEventListener('click', () => {
            tag.classList.toggle('selected');
            const value = tag.dataset.value;
            if (tag.classList.contains('selected')) {
                if (!State.selectedInterests.includes(value)) {
                    State.selectedInterests.push(value);
                }
            } else {
                State.selectedInterests = State.selectedInterests.filter(i => i !== value);
            }
        });
    });
    
    form?.addEventListener('submit', (e) => {
        e.preventDefault();
        const birthYear = parseInt(document.getElementById('birthYear').value);
        generatePersonalTimeline(birthYear, State.selectedInterests);
    });
}

function generatePersonalTimeline(birthYear, interests) {
    const currentYear = new Date().getFullYear();
    const container = document.getElementById('generatedTimeline');
    
    // Filter events
    let relevantEvents = CONFIG.TIMELINE_EVENTS.filter(event => 
        event.year >= birthYear && event.year <= currentYear
    );
    
    if (interests.length > 0) {
        relevantEvents = relevantEvents.filter(event => 
            event.categories.some(cat => interests.includes(cat))
        );
    }
    
    // Sort by year and take top events
    relevantEvents = relevantEvents
        .sort((a, b) => b.significance - a.significance)
        .slice(0, 8)
        .sort((a, b) => a.year - b.year);
    
    if (relevantEvents.length === 0) {
        showToast('No events found for your criteria. Try different interests!', 'error');
        return;
    }
    
    container.innerHTML = `
        <div class="timeline-intro-card">
            <h3>Your Journey Through History</h3>
            <p>Born in ${birthYear} • ${relevantEvents.length} major events during your lifetime</p>
        </div>
        <div class="personal-timeline">
            ${relevantEvents.map(event => {
                const age = event.year - birthYear;
                return `
                    <div class="personal-timeline-item">
                        <div class="personal-timeline-year">${event.year}</div>
                        <div class="personal-timeline-age">You were ${age} years old</div>
                        <h4 class="personal-timeline-title">${event.title}</h4>
                        <p class="personal-timeline-desc">${event.desc}</p>
                    </div>
                `;
            }).join('')}
        </div>
        <div class="timeline-share-section">
            <p>Share your timeline with friends</p>
            <button class="timeline-cta-btn" onclick="shareTimeline(${birthYear})">
                <i class="fas fa-share-alt"></i> Share My Timeline
            </button>
        </div>
    `;
    
    container.style.display = 'block';
    
    // Scroll to results
    container.scrollIntoView({ behavior: 'smooth', block: 'start' });
    
    showToast('Your personalized timeline is ready!', 'success');
}

function shareTimeline(birthYear) {
    const text = `I discovered the major historical events that happened during my lifetime on Chronos! Born in ${birthYear}, I've lived through incredible history. Check out your own timeline at chronos.app`;
    
    if (navigator.share) {
        navigator.share({
            title: 'My History Timeline - Chronos',
            text: text,
            url: window.location.href
        });
    } else {
        navigator.clipboard.writeText(text).then(() => {
            showToast('Timeline text copied to clipboard!', 'success');
        });
    }
}

// ==================== FUTURE PREDICTION MODE ====================
const PREDICTION_DATA = {
    tech: [
        { year: 2025, title: 'AI Revolution Peak', desc: 'Artificial Intelligence becomes indistinguishable from human intelligence in most tasks, transforming every industry.', confidence: 85 },
        { year: 2027, title: 'Quantum Computing Breakthrough', desc: 'First commercially viable quantum computers solve problems impossible for classical computers.', confidence: 70 },
        { year: 2030, title: 'Brain-Computer Interfaces', desc: 'Neural interfaces allow direct communication between human brains and devices.', confidence: 65 },
        { year: 2032, title: 'Fusion Energy Milestone', desc: 'Nuclear fusion achieves net positive energy output, beginning the clean energy revolution.', confidence: 60 },
        { year: 2035, title: 'Space Tourism Mainstream', desc: 'Orbital hotels and lunar bases become accessible to wealthy tourists.', confidence: 75 },
        { year: 2040, title: 'Humanoid Robots Everywhere', desc: 'Advanced humanoid robots become common household assistants worldwide.', confidence: 80 },
        { year: 2045, title: 'The Singularity', desc: 'AI surpasses human intelligence in all domains, marking a new era of human civilization.', confidence: 50 }
    ],
    country: [
        { year: 2026, title: 'New Global Power Balance', desc: 'Emerging economies reshape the geopolitical landscape with new alliances forming.', confidence: 80 },
        { year: 2028, title: 'Climate Migration Wave', desc: 'Rising sea levels and extreme weather trigger mass migrations affecting 100+ million people.', confidence: 90 },
        { year: 2030, title: 'Space Nations Emerge', desc: 'First permanent settlements on Moon and Mars declare autonomous governance.', confidence: 55 },
        { year: 2033, title: 'Resource Wars', desc: 'Competition for water, rare earth minerals, and arable land intensifies global tensions.', confidence: 70 },
        { year: 2035, title: 'Digital Borders', desc: 'Virtual nations with citizenship and governance challenge traditional nation-states.', confidence: 60 },
        { year: 2040, title: 'United Earth Federation', desc: 'Global cooperation on climate and space leads to a new world governance structure.', confidence: 45 }
    ],
    economy: [
        { year: 2025, title: 'Crypto Dollar Collapse', desc: 'Traditional fiat currencies face unprecedented challenges from decentralized alternatives.', confidence: 65 },
        { year: 2027, title: 'UBI Implementation', desc: 'Universal Basic Income becomes reality in major economies due to AI automation.', confidence: 70 },
        { year: 2029, title: 'Post-Scarcity Beginnings', desc: '3D printing and automation make basic goods nearly free in developed nations.', confidence: 55 },
        { year: 2031, title: 'Space Economy Boom', desc: 'Asteroid mining and space manufacturing create trillion-dollar new markets.', confidence: 75 },
        { year: 2034, title: 'Experience Economy Dominates', desc: 'Material goods lose value as experiences and digital assets become primary wealth.', confidence: 80 },
        { year: 2040, title: 'Resource-Based Economy', desc: 'AI-managed economies distribute resources based on need rather than money.', confidence: 40 }
    ]
};

function renderFuturePredictionPage() {
    return `
        <div class="prediction-page">
            <div class="prediction-hero">
                <h1><i class="fas fa-crystal-ball"></i> Future Prediction Mode</h1>
                <p>Explore possible futures based on current trends and emerging technologies. This is speculative entertainment based on expert forecasts.</p>
            </div>
            
            <div class="prediction-categories">
                <div class="prediction-category tech" data-category="tech">
                    <i class="fas fa-microchip"></i>
                    <h3>Technology</h3>
                    <p>AI, quantum computing, robotics, and innovation</p>
                </div>
                <div class="prediction-category country" data-category="country">
                    <i class="fas fa-globe-americas"></i>
                    <h3>Countries & Politics</h3>
                    <p>Geopolitics, nations, and global power shifts</p>
                </div>
                <div class="prediction-category economy" data-category="economy">
                    <i class="fas fa-chart-line"></i>
                    <h3>Economy</h3>
                    <p>Markets, currencies, and economic systems</p>
                </div>
            </div>
            
            <div class="prediction-results" id="predictionResults" style="display: none;"></div>
        </div>
    `;
}

function initFuturePredictionPage() {
    document.querySelectorAll('.prediction-category').forEach(cat => {
        cat.addEventListener('click', () => {
            const category = cat.dataset.category;
            showPredictions(category);
        });
    });
}

function showPredictions(category) {
    const container = document.getElementById('predictionResults');
    const predictions = PREDICTION_DATA[category] || [];
    const categoryNames = { tech: 'Technology', country: 'Countries & Politics', economy: 'Economy' };
    
    container.innerHTML = `
        <h2 style="font-family: var(--font-heading); margin-bottom: 2rem; text-align: center;">
            <i class="fas fa-arrow-trend-up"></i> ${categoryNames[category]} Predictions
        </h2>
        ${predictions.map(p => `
            <div class="prediction-card">
                <div class="prediction-year">${p.year}</div>
                <h3 class="prediction-title">${p.title}</h3>
                <p class="prediction-desc">${p.desc}</p>
                <span class="prediction-confidence">
                    <i class="fas fa-signal"></i> ${p.confidence}% confidence
                </span>
            </div>
        `).join('')}
        <div style="text-align: center; margin-top: 2rem; padding: 1.5rem; background: var(--bg-card); border-radius: 16px;">
            <p style="color: var(--text-muted); font-size: 0.9rem;">
                <i class="fas fa-info-circle"></i> These predictions are for entertainment purposes based on expert forecasts and trends.
            </p>
        </div>
    `;
    
    container.style.display = 'block';
    container.scrollIntoView({ behavior: 'smooth', block: 'start' });
}

// ==================== COMPARE LEGENDS MODE ====================
const COMPARISON_DATA = {
    'hitler-vs-napoleon': {
        left: { name: 'Adolf Hitler', era: '1889 - 1945', country: 'Germany', image: 'https://images.unsplash.com/photo-1550850839-8dc894ed385a?w=400&h=400&fit=crop', achievements: 'Led Nazi Germany, started WWII', impact: '65 million deaths, Holocaust', influence: '9/10 - Extreme negative influence', legacy: 'Universal symbol of evil' },
        right: { name: 'Napoleon Bonaparte', era: '1769 - 1821', country: 'France', image: 'https://images.unsplash.com/photo-1555662092-3696d6c8a56d?w=400&h=400&fit=crop', achievements: 'Emperor of France, Napoleonic Wars', impact: 'Modernized Europe, legal codes', influence: '8/10 - Mixed but significant', legacy: 'Military genius & reformer' },
        winner: 'napoleon',
        reason: 'Napoleon had lasting positive impacts on law and governance, while Hitler\'s legacy is purely destructive.'
    },
    'tesla-vs-edison': {
        left: { name: 'Nikola Tesla', era: '1856 - 1943', country: 'Serbia/USA', image: 'https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=400&h=400&fit=crop', achievements: 'AC electricity, wireless tech', impact: 'Powered the modern world', influence: '9/10 - Visionary inventor', legacy: 'Father of modern electricity' },
        right: { name: 'Thomas Edison', era: '1847 - 1931', country: 'USA', image: 'https://images.unsplash.com/photo-1497435334941-8c899ee9e8e9?w=400&h=400&fit=crop', achievements: 'Light bulb, phonograph, DC power', impact: 'Mass production of inventions', influence: '8/10 - Commercial genius', legacy: 'Prolific inventor & businessman' },
        winner: 'tesla',
        reason: 'Tesla\'s AC system powers the world today, while Edison\'s DC lost the war of currents.'
    },
    'mughals-vs-british': {
        left: { name: 'Mughal Empire', era: '1526 - 1857', country: 'Indian Subcontinent', image: 'https://images.unsplash.com/photo-1548013146-72479768bada?w=400&h=400&fit=crop', achievements: 'Taj Mahal, art, architecture', impact: 'Cultural synthesis, prosperity', influence: '8/10 - Cultural golden age', legacy: 'Indo-Islamic heritage' },
        right: { name: 'British Empire', era: '1583 - 1997', country: 'United Kingdom', image: 'https://images.unsplash.com/photo-1599707367072-cd6ada2bc375?w=400&h=400&fit=crop', achievements: 'Largest empire in history', impact: 'Colonization, industrial spread', influence: '9/10 - Global dominance', legacy: 'English language, common law' },
        winner: 'british',
        reason: 'The British Empire had a more lasting global impact, though both shaped modern India profoundly.'
    }
};

function renderCompareLegendsPage() {
    return `
        <div class="compare-page">
            <div class="compare-hero">
                <h1><i class="fas fa-balance-scale"></i> Compare Legends</h1>
                <p>Compare historical figures and empires side by side. See who had more impact, achievements, and lasting influence.</p>
            </div>
            
            <div class="compare-selector">
                <div class="compare-input-group">
                    <input type="text" class="compare-input" id="compareLeft" placeholder="First figure (e.g., Hitler)">
                    <span>VS</span>
                    <input type="text" class="compare-input" id="compareRight" placeholder="Second figure (e.g., Napoleon)">
                </div>
                <button class="compare-btn" id="startCompare">
                    <i class="fas fa-balance-scale"></i> Compare
                </button>
            </div>
            
            <div class="predefined-comparisons">
                <h3>Popular Comparisons</h3>
                <div class="comparison-chips">
                    <button class="comparison-chip" data-compare="hitler-vs-napoleon">
                        <i class="fas fa-crown"></i> Hitler vs Napoleon
                    </button>
                    <button class="comparison-chip" data-compare="tesla-vs-edison">
                        <i class="fas fa-lightbulb"></i> Tesla vs Edison
                    </button>
                    <button class="comparison-chip" data-compare="mughals-vs-british">
                        <i class="fas fa-landmark"></i> Mughals vs British
                    </button>
                    <button class="comparison-chip" data-compare="caesar-vs-alexander">
                        <i class="fas fa-shield-alt"></i> Caesar vs Alexander
                    </button>
                    <button class="comparison-chip" data-compare="einstein-vs-newton">
                        <i class="fas fa-atom"></i> Einstein vs Newton
                    </button>
                </div>
            </div>
            
            <div class="comparison-result" id="comparisonResult" style="display: none;"></div>
        </div>
    `;
}

function initCompareLegendsPage() {
    document.getElementById('startCompare')?.addEventListener('click', () => {
        const left = document.getElementById('compareLeft').value.trim().toLowerCase();
        const right = document.getElementById('compareRight').value.trim().toLowerCase();
        
        if (!left || !right) {
            showToast('Please enter both figures to compare', 'error');
            return;
        }
        
        const key = `${left}-vs-${right}`;
        const reverseKey = `${right}-vs-${left}`;
        
        if (COMPARISON_DATA[key]) {
            showComparison(key);
        } else if (COMPARISON_DATA[reverseKey]) {
            showComparison(reverseKey);
        } else {
            // Generate generic comparison
            generateGenericComparison(left, right);
        }
    });
    
    document.querySelectorAll('.comparison-chip').forEach(chip => {
        chip.addEventListener('click', () => {
            const compare = chip.dataset.compare;
            if (COMPARISON_DATA[compare]) {
                showComparison(compare);
            } else {
                showToast('Comparison coming soon!', 'info');
            }
        });
    });
}

function showComparison(key) {
    const data = COMPARISON_DATA[key];
    const container = document.getElementById('comparisonResult');
    
    container.innerHTML = `
        <div class="comparison-wrapper">
            <div class="vs-badge">VS</div>
            <div class="comparison-card">
                <div class="comparison-card-header">
                    <img src="${data.left.image}" alt="${data.left.name}">
                    <h3>${data.left.name}</h3>
                    <p>${data.left.era}</p>
                </div>
                <div class="comparison-card-body">
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Country</span>
                        <span class="comparison-stat-value">${data.left.country}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Achievements</span>
                        <span class="comparison-stat-value">${data.left.achievements}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Impact</span>
                        <span class="comparison-stat-value">${data.left.impact}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Influence</span>
                        <span class="comparison-stat-value">${data.left.influence}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Legacy</span>
                        <span class="comparison-stat-value">${data.left.legacy}</span>
                    </div>
                </div>
            </div>
            <div class="comparison-card">
                <div class="comparison-card-header">
                    <img src="${data.right.image}" alt="${data.right.name}">
                    <h3>${data.right.name}</h3>
                    <p>${data.right.era}</p>
                </div>
                <div class="comparison-card-body">
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Country</span>
                        <span class="comparison-stat-value">${data.right.country}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Achievements</span>
                        <span class="comparison-stat-value">${data.right.achievements}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Impact</span>
                        <span class="comparison-stat-value">${data.right.impact}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Influence</span>
                        <span class="comparison-stat-value">${data.right.influence}</span>
                    </div>
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Legacy</span>
                        <span class="comparison-stat-value">${data.right.legacy}</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="winner-banner">
            <h4><i class="fas fa-trophy"></i> Verdict</h4>
            <p>${data.reason}</p>
        </div>
    `;
    
    container.style.display = 'grid';
    container.scrollIntoView({ behavior: 'smooth', block: 'start' });
}

function generateGenericComparison(left, right) {
    const container = document.getElementById('comparisonResult');
    
    container.innerHTML = `
        <div class="comparison-wrapper">
            <div class="vs-badge">VS</div>
            <div class="comparison-card">
                <div class="comparison-card-header">
                    <div style="width: 120px; height: 120px; border-radius: 50%; background: linear-gradient(135deg, var(--accent-gold), var(--accent-purple)); display: flex; align-items: center; justify-content: center; margin: 0 auto 1rem; font-size: 3rem;">
                        <i class="fas fa-user"></i>
                    </div>
                    <h3>${left.charAt(0).toUpperCase() + left.slice(1)}</h3>
                </div>
                <div class="comparison-card-body">
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Status</span>
                        <span class="comparison-stat-value">Historical Figure</span>
                    </div>
                    <p style="color: var(--text-muted); text-align: center; padding: 2rem 0;">
                        Search for "${left}" to see full details
                    </p>
                </div>
            </div>
            <div class="comparison-card">
                <div class="comparison-card-header">
                    <div style="width: 120px; height: 120px; border-radius: 50%; background: linear-gradient(135deg, var(--accent-purple), var(--accent-blue)); display: flex; align-items: center; justify-content: center; margin: 0 auto 1rem; font-size: 3rem;">
                        <i class="fas fa-user"></i>
                    </div>
                    <h3>${right.charAt(0).toUpperCase() + right.slice(1)}</h3>
                </div>
                <div class="comparison-card-body">
                    <div class="comparison-stat">
                        <span class="comparison-stat-label">Status</span>
                        <span class="comparison-stat-value">Historical Figure</span>
                    </div>
                    <p style="color: var(--text-muted); text-align: center; padding: 2rem 0;">
                        Search for "${right}" to see full details
                    </p>
                </div>
            </div>
        </div>
        <div class="winner-banner">
            <h4><i class="fas fa-info-circle"></i> Compare Feature</h4>
            <p>Try our predefined comparisons or search for these figures to learn more about them!</p>
        </div>
    `;
    
    container.style.display = 'grid';
    container.scrollIntoView({ behavior: 'smooth', block: 'start' });
}

// ==================== ENHANCED LIBRARY FUNCTIONS ====================
function renderEnhancedLibraryPage() {
    const items = State.library;
    const collections = Object.keys(State.collections);
    const notes = State.notes;
    
    return `
        <div class="library-page">
            <div class="library-header">
                <h1 class="library-title"><i class="fas fa-bookmark"></i> My History Library</h1>
                <span class="library-count-badge">${items.length} saved</span>
            </div>
            
            <div class="library-tabs">
                <button class="library-tab active" data-tab="all">
                    <i class="fas fa-th-large"></i> All Saved
                </button>
                <button class="library-tab" data-tab="collections">
                    <i class="fas fa-folder"></i> Collections
                </button>
                <button class="library-tab" data-tab="notes">
                    <i class="fas fa-sticky-note"></i> My Notes (${notes.length})
                </button>
            </div>
            
            <div class="library-content" id="libraryContent">
                ${renderLibraryAll(items)}
            </div>
        </div>
    `;
}

function renderLibraryAll(items) {
    if (items.length === 0) {
        return `
            <div class="empty-library">
                <i class="fas fa-bookmark"></i>
                <h3>Your library is empty</h3>
                <p>Save topics you love to read them later</p>
                <button class="empty-library-btn" onclick="Router.navigate('explore')">
                    <i class="fas fa-compass"></i> Explore Topics
                </button>
            </div>
        `;
    }
    
    return `
        <div class="library-grid">
            ${items.map((item, index) => `
                <div class="library-card" style="animation-delay: ${index * 0.05}s">
                    <div class="library-card-image" style="background-image: url('${item.image}')"></div>
                    <div class="library-card-content">
                        ${item.collection ? `<div class="library-card-collection"><i class="fas fa-folder"></i> ${item.collection}</div>` : ''}
                        <h3 class="library-card-title">${item.title}</h3>
                        <p class="library-card-era">${item.era}</p>
                        <div class="library-card-actions">
                            <button class="library-card-btn read-btn" data-slug="${item.slug}">
                                <i class="fas fa-book-open"></i> Read
                            </button>
                            <button class="library-card-btn" onclick="openNoteModal('${item.slug}', '${item.title}')">
                                <i class="fas fa-sticky-note"></i>
                            </button>
                            <button class="library-card-btn" onclick="openCollectionModal('${item.slug}')">
                                <i class="fas fa-folder-plus"></i>
                            </button>
                            <button class="library-card-btn remove" data-slug="${item.slug}">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                </div>
            `).join('')}
        </div>
    `;
}

function renderCollections() {
    const defaultCollections = [
        { id: 'war', name: 'War & Battles', icon: 'fa-shield-alt', color: 'war' },
        { id: 'business', name: 'Business', icon: 'fa-briefcase', color: 'business' },
        { id: 'kings', name: 'Kings & Royals', icon: 'fa-crown', color: 'kings' },
        { id: 'dark', name: 'Dark History', icon: 'fa-moon', color: 'dark' }
    ];
    
    const customCollections = Object.keys(State.collections).filter(c => !defaultCollections.find(d => d.id === c));
    
    return `
        <div class="collections-grid">
            ${defaultCollections.map(col => {
                const count = State.getItemsByCollection(col.id).length;
                return `
                    <div class="collection-card ${col.color}" onclick="showCollectionItems('${col.id}')">
                        <i class="fas ${col.icon}"></i>
                        <h3>${col.name}</h3>
                        <p>${count} items</p>
                    </div>
                `;
            }).join('')}
            ${customCollections.map(col => {
                const count = State.getItemsByCollection(col).length;
                return `
                    <div class="collection-card custom" onclick="showCollectionItems('${col}')">
                        <i class="fas fa-folder"></i>
                        <h3>${col}</h3>
                        <p>${count} items</p>
                    </div>
                `;
            }).join('')}
        </div>
        <div style="margin-top: 2rem; text-align: center;">
            <button class="timeline-cta-btn" onclick="createNewCollection()">
                <i class="fas fa-plus"></i> Create New Collection
            </button>
        </div>
    `;
}

function renderNotes() {
    const notes = State.notes;
    
    if (notes.length === 0) {
        return `
            <div class="empty-collection">
                <i class="fas fa-sticky-note"></i>
                <h4>No notes yet</h4>
                <p>Add notes to your saved topics</p>
            </div>
        `;
    }
    
    return `
        <div class="notes-section">
            ${notes.map(note => `
                <div class="note-card">
                    <div class="note-header">
                        <span class="note-title">${note.title}</span>
                        <span class="note-date">${new Date(note.createdAt).toLocaleDateString()}</span>
                    </div>
                    <p class="note-content">${note.content}</p>
                    <div class="note-actions">
                        <button class="note-btn" onclick="Router.navigate('history', { slug: '${note.itemSlug}' })">
                            <i class="fas fa-book-open"></i> View Topic
                        </button>
                        <button class="note-btn" onclick="deleteNote('${note.id}')">
                            <i class="fas fa-trash"></i> Delete
                        </button>
                    </div>
                </div>
            `).join('')}
        </div>
    `;
}

function showCollectionItems(collectionId) {
    const items = State.getItemsByCollection(collectionId);
    const container = document.getElementById('libraryContent');
    
    if (items.length === 0) {
        container.innerHTML = `
            <div class="empty-collection">
                <i class="fas fa-folder-open"></i>
                <h4>No items in this collection</h4>
                <p>Add items to get started</p>
                <button class="empty-library-btn" onclick="Router.navigate('explore')" style="margin-top: 1rem;">
                    <i class="fas fa-compass"></i> Explore
                </button>
            </div>
        `;
        return;
    }
    
    container.innerHTML = `
        <div style="margin-bottom: 1.5rem;">
            <button class="note-btn" onclick="showLibraryTab('collections')">
                <i class="fas fa-arrow-left"></i> Back to Collections
            </button>
        </div>
        <div class="library-grid">
            ${items.map((item, index) => `
                <div class="library-card" style="animation-delay: ${index * 0.05}s">
                    <div class="library-card-image" style="background-image: url('${item.image}')"></div>
                    <div class="library-card-content">
                        <h3 class="library-card-title">${item.title}</h3>
                        <p class="library-card-era">${item.era}</p>
                        <div class="library-card-actions">
                            <button class="library-card-btn read-btn" data-slug="${item.slug}">
                                <i class="fas fa-book-open"></i> Read
                            </button>
                            <button class="library-card-btn remove" data-slug="${item.slug}">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                </div>
            `).join('')}
        </div>
    `;
}

function showLibraryTab(tab) {
    const container = document.getElementById('libraryContent');
    document.querySelectorAll('.library-tab').forEach(t => t.classList.remove('active'));
    document.querySelector(`.library-tab[data-tab="${tab}"]`)?.classList.add('active');
    
    switch(tab) {
        case 'all':
            container.innerHTML = renderLibraryAll(State.library);
            break;
        case 'collections':
            container.innerHTML = renderCollections();
            break;
        case 'notes':
            container.innerHTML = renderNotes();
            break;
    }
}

function openNoteModal(slug, title) {
    State.currentNoteItem = { slug, title };
    document.getElementById('noteTitle').value = `Notes on ${title}`;
    document.getElementById('noteContent').value = '';
    document.getElementById('noteModal').classList.add('active');
}

function closeNoteModal() {
    document.getElementById('noteModal').classList.remove('active');
    State.currentNoteItem = null;
}

function saveNote() {
    const title = document.getElementById('noteTitle').value.trim();
    const content = document.getElementById('noteContent').value.trim();
    
    if (!title || !content) {
        showToast('Please enter both title and content', 'error');
        return;
    }
    
    if (!State.currentNoteItem) return;
    
    State.addNote({
        title,
        content,
        itemSlug: State.currentNoteItem.slug,
        itemTitle: State.currentNoteItem.title
    });
    
    closeNoteModal();
    showToast('Note saved!', 'success');
}

function deleteNote(id) {
    if (confirm('Delete this note?')) {
        State.removeNote(id);
        showLibraryTab('notes');
        showToast('Note deleted', 'success');
    }
}

function openCollectionModal(slug) {
    State.currentCollectionItem = slug;
    document.querySelectorAll('.collection-tag').forEach(t => t.classList.remove('selected'));
    document.getElementById('newCollectionName').value = '';
    document.getElementById('collectionModal').classList.add('active');
}

function closeCollectionModal() {
    document.getElementById('collectionModal').classList.remove('active');
    State.currentCollectionItem = null;
}

function saveToCollection() {
    const selectedTag = document.querySelector('.collection-tag.selected');
    const newName = document.getElementById('newCollectionName').value.trim();
    
    let collection = null;
    if (selectedTag) {
        collection = selectedTag.dataset.collection;
    } else if (newName) {
        collection = newName.toLowerCase().replace(/\s+/g, '-');
    }
    
    if (!collection) {
        showToast('Please select or create a collection', 'error');
        return;
    }
    
    const item = State.library.find(i => i.slug === State.currentCollectionItem);
    if (item) {
        item.collection = collection;
        if (!State.collections[collection]) {
            State.collections[collection] = [];
        }
        State.collections[collection].push(item.slug);
        State.saveLibrary();
        State.saveCollections();
        showToast(`Added to ${collection}!`, 'success');
    }
    
    closeCollectionModal();
}

function createNewCollection() {
    const name = prompt('Enter collection name:');
    if (name) {
        const key = name.toLowerCase().replace(/\s+/g, '-');
        if (!State.collections[key]) {
            State.collections[key] = [];
            State.saveCollections();
            showLibraryTab('collections');
            showToast('Collection created!', 'success');
        } else {
            showToast('Collection already exists', 'error');
        }
    }
}

// ==================== SHARE MODAL ====================
function openShareModal(data) {
    const modal = document.getElementById('shareModal');
    const preview = document.getElementById('sharePreview');
    
    // Generate card preview HTML
    preview.innerHTML = `
        <div class="share-card-preview" id="shareCardElement">
            <div class="share-card-logo">
                <i class="fas fa-hourglass-half"></i> CHRONOS
            </div>
            <div class="share-card-content">
                <div class="share-card-year">${data.year}</div>
                <h3 class="share-card-title">${data.title}</h3>
                <p class="share-card-desc">${data.extract.replace(/<[^>]*>/g, '').substring(0, 120)}...</p>
            </div>
            <div class="share-card-footer">
                chronos.app • Journey Through Time
            </div>
        </div>
    `;
    
    modal.classList.add('active');
    
    // Setup download button
    document.getElementById('downloadCard').onclick = () => downloadShareCard(data);
    
    // Setup copy link button
    document.getElementById('copyLink').onclick = () => {
        const link = `${window.location.origin}${window.location.pathname}#/history/${data.slug}`;
        navigator.clipboard.writeText(link).then(() => {
            showToast('Link copied to clipboard!', 'success');
        });
    };
    
    // Setup social share buttons
    document.querySelectorAll('.share-btn').forEach(btn => {
        btn.onclick = () => {
            const platform = btn.dataset.platform;
            const url = encodeURIComponent(`${window.location.origin}${window.location.pathname}#/history/${data.slug}`);
            const text = encodeURIComponent(`Check out "${data.title}" on Chronos - Journey Through Time`);
            
            let shareUrl = '';
            switch(platform) {
                case 'twitter':
                    shareUrl = `https://twitter.com/intent/tweet?text=${text}&url=${url}`;
                    break;
                case 'facebook':
                    shareUrl = `https://www.facebook.com/sharer/sharer.php?u=${url}`;
                    break;
                case 'whatsapp':
                    shareUrl = `https://wa.me/?text=${text}%20${url}`;
                    break;
                case 'telegram':
                    shareUrl = `https://t.me/share/url?url=${url}&text=${text}`;
                    break;
            }
            
            if (shareUrl) {
                window.open(shareUrl, '_blank', 'width=600,height=400');
            }
        };
    });
}

async function downloadShareCard(data) {
    const cardElement = document.getElementById('shareCardElement');
    
    try {
        showLoading('Generating your card...');
        
        const canvas = await html2canvas(cardElement, {
            scale: 2,
            backgroundColor: '#0a0a0f',
            logging: false
        });
        
        const link = document.createElement('a');
        link.download = `chronos-${data.slug}.png`;
        link.href = canvas.toDataURL('image/png');
        link.click();
        
        hideLoading();
        showToast('Card downloaded!', 'success');
    } catch (error) {
        hideLoading();
        showToast('Failed to generate card. Please try again.', 'error');
        console.error('Card generation error:', error);
    }
}

function closeShareModal() {
    document.getElementById('shareModal').classList.remove('active');
}

// ==================== AUTH MODAL ====================
function openAuthModal() {
    document.getElementById('authModal').classList.add('active');
}

function closeAuthModal() {
    document.getElementById('authModal').classList.remove('active');
}

// ==================== AUDIO FUNCTIONS ====================
function playAudio(text, title) {
    if (State.speechSynth.speaking) {
        State.speechSynth.cancel();
    }
    
    let voices = State.speechSynth.getVoices();
    
    if (voices.length === 0) {
        State.speechSynth.onvoiceschanged = () => {
            voices = State.speechSynth.getVoices();
            startSpeech(text, title, voices);
        };
    } else {
        startSpeech(text, title, voices);
    }
}

function startSpeech(text, title, voices) {
    const preferredVoice = voices.find(v => v.name.includes('Google US English')) ||
                          voices.find(v => v.name.includes('Samantha')) ||
                          voices.find(v => v.lang === 'en-US') ||
                          voices[0];
    
    const utterance = new SpeechSynthesisUtterance(text);
    utterance.voice = preferredVoice;
    utterance.rate = 0.9;
    utterance.pitch = 1;
    utterance.volume = 1;
    
    State.currentUtterance = utterance;
    
    const player = document.getElementById('audioPlayer');
    const audioTitle = document.getElementById('audioTitle');
    const playPauseBtn = document.getElementById('audioPlayPause');
    
    audioTitle.textContent = title.substring(0, 25) + (title.length > 25 ? '...' : '');
    player.classList.add('active');
    State.isPlaying = true;
    playPauseBtn.innerHTML = '<i class="fas fa-pause"></i>';
    
    utterance.onend = () => {
        State.isPlaying = false;
        playPauseBtn.innerHTML = '<i class="fas fa-play"></i>';
    };
    
    utterance.onerror = (e) => {
        console.error('Speech error:', e);
        showToast('Audio playback failed. Please try again.', 'error');
        stopAudio();
    };
    
    State.speechSynth.speak(utterance);
}

function stopAudio() {
    if (State.speechSynth.speaking) {
        State.speechSynth.cancel();
    }
    State.isPlaying = false;
    document.getElementById('audioPlayer').classList.remove('active');
}

// ==================== UI HELPERS ====================
function showToast(message, type = 'success') {
    const container = document.getElementById('toastContainer');
    const toast = document.createElement('div');
    toast.className = `toast ${type}`;
    toast.innerHTML = `
        <i class="fas ${type === 'success' ? 'fa-check-circle' : type === 'error' ? 'fa-exclamation-circle' : 'fa-info-circle'}"></i>
        <span>${message}</span>
    `;
    
    container.appendChild(toast);
    
    gsap.fromTo(toast, 
        { opacity: 0, x: 100 },
        { opacity: 1, x: 0, duration: 0.3, ease: 'power2.out' }
    );
    
    setTimeout(() => {
        gsap.to(toast, {
            opacity: 0,
            x: 100,
            duration: 0.3,
            onComplete: () => toast.remove()
        });
    }, 3000);
}

function showLoading(subtext = '') {
    const overlay = document.getElementById('loadingOverlay');
    const subtextEl = document.getElementById('loadingSubtext');
    if (subtext) subtextEl.textContent = subtext;
    overlay.classList.add('active');
}

function hideLoading() {
    document.getElementById('loadingOverlay').classList.remove('active');
}

function updateLibraryCount() {
    const count = State.library.length;
    const badge = document.getElementById('libraryCount');
    if (badge) {
        badge.textContent = count;
        gsap.fromTo(badge, 
            { scale: 1.3 },
            { scale: 1, duration: 0.3, ease: 'back.out' }
        );
    }
}

function initParticles() {
    const container = document.getElementById('particles');
    if (!container) return;
    for (let i = 0; i < 30; i++) {
        const particle = document.createElement('div');
        particle.className = 'particle';
        particle.style.left = Math.random() * 100 + '%';
        particle.style.animationDelay = Math.random() * 20 + 's';
        particle.style.animationDuration = (15 + Math.random() * 10) + 's';
        container.appendChild(particle);
    }
}

// ==================== INITIALIZATION ====================
document.addEventListener('DOMContentLoaded', () => {
    try {
        // Initialize Firebase (with error handling)
        try {
            initFirebase();
        } catch (e) {
            console.warn('Firebase init failed, continuing without auth:', e);
        }
        
        // Load library from storage
        State.loadFromStorage();
        
        // Initialize particles
        initParticles();
        
        // Initialize router
        Router.init();
        
        // Render home page immediately if no hash
        if (!window.location.hash || window.location.hash === '#/' || window.location.hash === '') {
            const app = document.getElementById('app');
            if (app) {
                app.innerHTML = renderHomePage();
                initHomePage();
            }
        }
    } catch (error) {
        console.error('Initialization error:', error);
        // Fallback: render home page
        const app = document.getElementById('app');
        if (app) {
            app.innerHTML = renderHomePage();
            initHomePage();
        }
    }
    
    // Audio player controls
    document.getElementById('audioPlayPause')?.addEventListener('click', () => {
        const btn = document.getElementById('audioPlayPause');
        
        if (State.speechSynth.speaking) {
            if (State.isPlaying) {
                State.speechSynth.pause();
                State.isPlaying = false;
                btn.innerHTML = '<i class="fas fa-play"></i>';
            } else {
                State.speechSynth.resume();
                State.isPlaying = true;
                btn.innerHTML = '<i class="fas fa-pause"></i>';
            }
        }
    });
    
    document.getElementById('audioStop')?.addEventListener('click', stopAudio);
    document.getElementById('audioClose')?.addEventListener('click', stopAudio);
    
    // Modal controls
    document.getElementById('closeAuthModal')?.addEventListener('click', closeAuthModal);
    document.getElementById('closeShareModal')?.addEventListener('click', closeShareModal);
    
    // Auth buttons
    document.getElementById('googleSignIn')?.addEventListener('click', signInWithGoogle);
    document.getElementById('guestSignIn')?.addEventListener('click', signInAsGuest);
    
    // Login button (using event delegation for dynamically added button)
    document.addEventListener('click', (e) => {
        const loginBtn = e.target.closest('#loginBtn');
        if (loginBtn) {
            openAuthModal();
        }
    });
    
    // Mobile menu
    document.getElementById('mobileMenuBtn')?.addEventListener('click', () => {
        document.getElementById('mobileMenu').classList.toggle('active');
    });
    
    // Side menu
    const sideMenu = document.getElementById('sideMenu');
    const sideMenuOverlay = document.getElementById('sideMenuOverlay');
    
    function openSideMenu() {
        sideMenu?.classList.add('active');
        sideMenuOverlay?.classList.add('active');
    }
    
    function closeSideMenu() {
        sideMenu?.classList.remove('active');
        sideMenuOverlay?.classList.remove('active');
    }
    
    document.getElementById('closeSideMenu')?.addEventListener('click', closeSideMenu);
    sideMenuOverlay?.addEventListener('click', closeSideMenu);
    
    // Side menu navigation
    document.querySelectorAll('.side-menu-item[data-route]').forEach(item => {
        item.addEventListener('click', (e) => {
            e.preventDefault();
            const route = item.dataset.route;
            Router.navigate(route);
            closeSideMenu();
        });
    });
    
    // Library actions (delegated)
    document.addEventListener('click', (e) => {
        const removeBtn = e.target.closest('.library-card-btn.remove');
        const readBtn = e.target.closest('.library-card-btn.read-btn');
        
        if (removeBtn) {
            const slug = removeBtn.dataset.slug;
            State.removeFromLibrary(slug);
            showToast('Removed from library', 'success');
            Router.navigate('library');
        }
        
        if (readBtn) {
            const slug = readBtn.dataset.slug;
            Router.navigate('history', { slug });
        }
    });
    
    // Nav scroll effect
    window.addEventListener('scroll', () => {
        const nav = document.getElementById('mainNav');
        if (window.scrollY > 50) {
            nav.classList.add('scrolled');
        } else {
            nav.classList.remove('scrolled');
        }
    });
    
    // Close modals on backdrop click
    document.querySelectorAll('.modal').forEach(modal => {
        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                modal.classList.remove('active');
            }
        });
    });
    
    // Note modal
    document.getElementById('closeNoteModal')?.addEventListener('click', closeNoteModal);
    document.getElementById('saveNoteBtn')?.addEventListener('click', saveNote);
    
    // Collection modal
    document.getElementById('closeCollectionModal')?.addEventListener('click', closeCollectionModal);
    document.getElementById('saveToCollectionBtn')?.addEventListener('click', saveToCollection);
    
    // Collection tag selection
    document.querySelectorAll('.collection-tag').forEach(tag => {
        tag.addEventListener('click', () => {
            document.querySelectorAll('.collection-tag').forEach(t => t.classList.remove('selected'));
            tag.classList.add('selected');
            document.getElementById('newCollectionName').value = '';
        });
    });
    
    // Library tabs
    document.addEventListener('click', (e) => {
        const tab = e.target.closest('.library-tab');
        if (tab) {
            const tabName = tab.dataset.tab;
            showLibraryTab(tabName);
        }
    });
});

// Console easter egg
console.log('%c 🏛️ CHRONOS 2.0 ', 'background: linear-gradient(135deg, #d4af37, #8b5cf6); color: #0a0a0f; font-size: 24px; font-weight: bold; padding: 10px 20px; border-radius: 10px;');
console.log('%c Journey Through Time - Premium History Experience', 'color: #d4af37; font-size: 14px;');
console.log('%c Features: Firebase Auth • Daily History • Timeline Generator • Share Cards', 'color: #a0a0b0; font-size: 12px;');
