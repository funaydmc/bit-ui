<script lang="ts">
	export let variant: 'primary' | 'secondary' | 'danger' = 'primary';
	export let size: 'sm' | 'md' | 'lg' = 'md';
	export let disabled = false;
</script>

<button 
	class="btn btn--{variant} btn--{size}" 
	class:btn--disabled={disabled} 
	{disabled}
	on:click
>
	<slot />
</button>

<style>
	.btn {
		display: inline-flex;
		align-items: center;
		justify-content: center;
		border: none;
		border-radius: 6px;
		font-weight: 500;
		cursor: pointer;
		transition: all 0.2s;
	}
	
	.btn:disabled {
		cursor: not-allowed;
		opacity: 0.6;
	}
	
	/* Sizes */
	.btn--sm {
		padding: 0.5rem 1rem;
		font-size: 0.875rem;
	}
	
	.btn--md {
		padding: 0.75rem 1.5rem;
		font-size: 1rem;
	}
	
	.btn--lg {
		padding: 1rem 2rem;
		font-size: 1.125rem;
	}
	
	/* Variants */
	.btn--primary {
		background-color: #3b82f6;
		color: white;
	}
	
	.btn--primary:hover:not(:disabled) {
		background-color: #2563eb;
	}
	
	.btn--secondary {
		background-color: #f3f4f6;
		color: #374151;
		border: 1px solid #d1d5db;
	}
	
	.btn--secondary:hover:not(:disabled) {
		background-color: #e5e7eb;
	}
	
	.btn--danger {
		background-color: #ef4444;
		color: white;
	}
	
	.btn--danger:hover:not(:disabled) {
		background-color: #dc2626;
	}
</style>