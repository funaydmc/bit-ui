<script>
	import { Button } from '$lib';
</script>

<main class="container">
	<h1>Bit UI Component Library</h1>
	<p>A modern Svelte component library with TypeScript support.</p>
	
	<section class="demo-section">
		<h2>Button Component</h2>
		
		<div class="demo-group">
			<h3>Variants</h3>
			<div class="button-grid">
				<Button variant="primary">Primary Button</Button>
				<Button variant="secondary">Secondary Button</Button>
				<Button variant="danger">Danger Button</Button>
			</div>
		</div>
		
		<div class="demo-group">
			<h3>Sizes</h3>
			<div class="button-grid">
				<Button size="sm">Small</Button>
				<Button size="md">Medium</Button>
				<Button size="lg">Large</Button>
			</div>
		</div>
		
		<div class="demo-group">
			<h3>States</h3>
			<div class="button-grid">
				<Button>Normal</Button>
				<Button disabled>Disabled</Button>
			</div>
		</div>
	</section>
	
	<section class="usage-section">
		<h2>Usage</h2>
		<pre><code>npm install bit-ui</code></pre>
		<pre><code>import { Button } from 'bit-ui';</code></pre>
	</section>
</main>

<style>
	.container {
		max-width: 1200px;
		margin: 0 auto;
		padding: 2rem;
		font-family: system-ui, sans-serif;
	}
	
	h1 {
		color: #1f2937;
		margin-bottom: 1rem;
	}
	
	.demo-section {
		margin: 3rem 0;
	}
	
	.demo-group {
		margin: 2rem 0;
	}
	
	h2 {
		color: #374151;
		margin-bottom: 1rem;
		border-bottom: 2px solid #e5e7eb;
		padding-bottom: 0.5rem;
	}
	
	h3 {
		color: #6b7280;
		margin-bottom: 1rem;
		font-size: 1.1rem;
	}
	
	.button-grid {
		display: flex;
		gap: 1rem;
		flex-wrap: wrap;
		margin: 1rem 0;
	}
	
	.usage-section {
		background: #f9fafb;
		border: 1px solid #e5e7eb;
		border-radius: 8px;
		padding: 2rem;
		margin: 3rem 0;
	}
	
	pre {
		background: #1f2937;
		color: #f9fafb;
		padding: 1rem;
		border-radius: 6px;
		margin: 1rem 0;
		overflow-x: auto;
	}
	
	code {
		font-family: 'Monaco', 'Consolas', monospace;
	}
</style>
