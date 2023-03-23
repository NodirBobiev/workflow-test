<script>
	// // Import the functions you need from the SDKs you need
	// import { initializeApp } from "firebase/analytics";
	// import { getAnalytics } from "firebase/analytics";
	// // TODO: Add SDKs for Firebase products that you want to use
	// // https://firebase.google.com/docs/web/setup#available-libraries

	// // Your web app's Firebase configuration
	// // For Firebase JS SDK v7.20.0 and later, measurementId is optional
	// const firebaseConfig = {
	// 	apiKey: "AIzaSyAUdGdMJPq1SV4Bu3Mr5A0Pe27JZUSR7Eo",
	// 	authDomain: "workflow-test-84377.firebaseapp.com",
	// 	projectId: "workflow-test-84377",
	// 	storageBucket: "workflow-test-84377.appspot.com",
	// 	messagingSenderId: "92363187900",
	// 	appId: "1:92363187900:web:0ea8c131a0ce888da4d2b9",
	// 	measurementId: "G-V8FPMYPHPN"
	// };

	// // Initialize Firebase
	// const app = initializeApp(firebaseConfig);
	// const analytics = getAnalytics(app);

	import Header from './Header.svelte';
	import './styles.css';

</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	footer a {
		font-weight: bold;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
