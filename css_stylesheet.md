/* STYLES */

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    background-color: #f4f6f8;
    color: #1a1a1a;
    line-height: 1.5;
    padding: 20px;
}

header {
    margin-bottom: 20px;
    text-align: center;
}

header h1 {
    font-size: 1.8rem;
    color: #0d253f;
}

.subtitle {
    color: #555;
    font-size: 0.95rem;
}

.container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    max-width: 1200px;
    margin: 0 auto;
}

@media (max-width: 768px) {
    .container {
        grid-template-columns: 1fr;
    }
}

.card {
    background: #ffffff;
    border-radius: 8px;
    border: 1px solid #e1e4e8;
    padding: 20px;
    display: flex;
    flex-direction: column;
    box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}

.card-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 12px;
}

.card-header h2 {
    font-size: 1.25rem;
}

.controls {
    display: flex;
    gap: 8px;
}

.btn {
    padding: 8px 14px;
    border: none;
    border-radius: 6px;
    font-size: 0.9rem;
    font-weight: 600;
    cursor: pointer;
    transition: background-color 0.2s;
}

.btn.primary {
    background-color: #0066cc;
    color: white;
}
.btn.primary:hover:not(:disabled) {
    background-color: #0052a3;
}

.btn.danger {
    background-color: #d9381e;
    color: white;
}
.btn.danger:hover:not(:disabled) {
    background-color: #b82c16;
}

.btn.secondary {
    background-color: #e2e8f0;
    color: #1a202c;
    margin-top: 12px;
}
.btn.secondary:hover {
    background-color: #cbd5e0;
}

.btn.danger-outline {
    background-color: transparent;
    border: 1px solid #d9381e;
    color: #d9381e;
}
.btn.danger-outline:hover {
    background-color: #fff5f5;
}

.btn:disabled {
    opacity: 0.5;
    cursor: not-allowed;
}

.status-indicator {
    font-size: 0.85rem;
    color: #4a5568;
    margin-bottom: 10px;
    font-weight: 500;
}

.status-indicator.error {
    color: #d9381e;
}

.caption-display {
    min-height: 250px;
    max-height: 400px;
    overflow-y: auto;
    border: 1px solid #e2e8f0;
    border-radius: 6px;
    padding: 12px;
    background-color: #fafafa;
    font-size: 1.1rem;
    line-height: 1.6;
}

.placeholder {
    color: #a0aec0;
    font-style: italic;
}

.final-text {
    color: #1a202c;
}

.interim-text {
    color: #718096;
    font-style: italic;
}

textarea#notes-input {
    width: 100%;
    min-height: 300px;
    padding: 12px;
    border: 1px solid #e2e8f0;
    border-radius: 6px;
    font-family: inherit;
    font-size: 1rem;
    line-height: 1.5;
    resize: vertical;
}

textarea#notes-input:focus {
    outline: none;
    border-color: #0066cc;
}