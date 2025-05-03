<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ImageCompressorPro - Beautiful Image Compression Tool</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #4361ee;
            --primary-light: #4895ef;
            --secondary: #3f37c9;
            --accent: #f72585;
            --dark: #1a1a2e;
            --light: #f8f9fa;
            --gray: #6c757d;
            --success: #4cc9f0;
            --warning: #f8961e;
            --danger: #ef233c;
            
            --shadow-sm: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
            --shadow-md: 0 4px 6px rgba(0,0,0,0.1), 0 1px 3px rgba(0,0,0,0.08);
            --shadow-lg: 0 10px 25px rgba(0,0,0,0.1), 0 5px 10px rgba(0,0,0,0.05);
            --shadow-xl: 0 20px 40px rgba(0,0,0,0.15);
            
            --radius-sm: 8px;
            --radius-md: 12px;
            --radius-lg: 16px;
            --radius-full: 9999px;
            
            --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f5f7ff;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: white;
            box-shadow: var(--shadow-sm);
            position: sticky;
            top: 0;
            z-index: 100;
            padding: 15px 0;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
        }
        
        .logo-icon {
            width: 36px;
            height: 36px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: var(--radius-sm);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 18px;
        }
        
        .logo-text {
            font-size: 1.5rem;
            font-weight: 700;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--gray);
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }
        
        nav ul li a:hover {
            color: var(--primary);
        }
        
        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: var(--transition);
        }
        
        nav ul li a:hover::after {
            width: 100%;
        }
        
        /* Main Content */
        .main-content {
            margin: 40px 0;
            background: white;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-md);
            overflow: hidden;
            transition: var(--transition);
        }
        
        .main-content:hover {
            box-shadow: var(--shadow-lg);
        }
        
        .hero {
            padding: 40px;
            background: linear-gradient(135deg, rgba(67, 97, 238, 0.1), rgba(63, 55, 201, 0.1));
            text-align: center;
            border-bottom: 1px solid rgba(0,0,0,0.05);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .description {
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto 25px;
            font-size: 1.1rem;
        }
        
        .features {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        
        .feature {
            background: white;
            padding: 12px 20px;
            border-radius: var(--radius-sm);
            box-shadow: var(--shadow-sm);
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.9rem;
            color: var(--primary);
        }
        
        .feature i {
            color: var(--success);
        }
        
        /* Compressor */
        .compressor-container {
            padding: 30px;
        }
        
        .upload-area {
            border: 2px dashed rgba(67, 97, 238, 0.3);
            border-radius: var(--radius-md);
            padding: 50px 20px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
            background: rgba(67, 97, 238, 0.03);
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
        }
        
        .upload-area:hover {
            border-color: var(--primary);
            background: rgba(67, 97, 238, 0.05);
        }
        
        .upload-area.active {
            border-color: var(--primary);
            background: rgba(67, 97, 238, 0.1);
        }
        
        .upload-icon {
            font-size: 3.5rem;
            color: var(--primary);
            margin-bottom: 15px;
            transition: var(--transition);
        }
        
        .upload-area:hover .upload-icon {
            transform: translateY(-5px);
        }
        
        .upload-text {
            font-size: 1.3rem;
            margin-bottom: 10px;
            font-weight: 500;
            color: var(--dark);
        }
        
        .upload-subtext {
            color: var(--gray);
            font-size: 0.95rem;
        }
        
        #file-input {
            display: none;
        }
        
        .file-preview {
            display: none;
            margin-bottom: 30px;
            animation: fadeIn 0.5s ease;
        }
        
        .file-preview img {
            max-width: 200px;
            max-height: 200px;
            border-radius: var(--radius-sm);
            box-shadow: var(--shadow-sm);
        }
        
        .file-info {
            margin-top: 10px;
            font-size: 0.9rem;
            color: var(--gray);
        }
        
        /* Controls */
        .controls {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }
        
        .control-group {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
        
        .control-header {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .control-header i {
            color: var(--primary);
            font-size: 1.2rem;
        }
        
        label {
            font-weight: 600;
            color: var(--dark);
            font-size: 1.1rem;
        }
        
        .control-description {
            color: var(--gray);
            font-size: 0.9rem;
            margin-bottom: 5px;
        }
        
        .slider-container {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .slider-value {
            min-width: 45px;
            text-align: center;
            font-weight: 600;
            color: var(--primary);
            background: rgba(67, 97, 238, 0.1);
            padding: 5px 10px;
            border-radius: var(--radius-sm);
        }
        
        input[type="range"] {
            flex-grow: 1;
            height: 8px;
            -webkit-appearance: none;
            background: rgba(67, 97, 238, 0.1);
            border-radius: var(--radius-full);
            outline: none;
            transition: var(--transition);
        }
        
        input[type="range"]:hover {
            background: rgba(67, 97, 238, 0.2);
        }
        
        input[type="range"]::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 22px;
            height: 22px;
            background: var(--primary);
            border-radius: 50%;
            cursor: pointer;
            transition: var(--transition);
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }
        
        input[type="range"]::-webkit-slider-thumb:hover {
            transform: scale(1.1);
            background: var(--accent);
        }
        
        .format-options {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .format-option {
            padding: 10px 20px;
            border: 1px solid rgba(67, 97, 238, 0.3);
            border-radius: var(--radius-sm);
            cursor: pointer;
            transition: var(--transition);
            font-size: 0.95rem;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .format-option:hover {
            border-color: var(--primary);
            color: var(--primary);
            transform: translateY(-2px);
        }
        
        .format-option.selected {
            background: var(--primary);
            color: white;
            border-color: var(--primary);
            box-shadow: 0 4px 10px rgba(67, 97, 238, 0.2);
        }
        
        .format-option i {
            font-size: 1.1rem;
        }
        
        .buttons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .button {
            padding: 14px 28px;
            border: none;
            border-radius: var(--radius-sm);
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            font-size: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
        }
        
        .button-primary {
            background: var(--primary);
            color: white;
            box-shadow: 0 4px 10px rgba(67, 97, 238, 0.3);
        }
        
        .button-primary:hover {
            background: var(--secondary);
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(67, 97, 238, 0.4);
        }
        
        .button-primary:disabled {
            background: var(--gray);
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
            opacity: 0.7;
        }
        
        .button-secondary {
            background: white;
            color: var(--primary);
            border: 1px solid var(--primary);
        }
        
        .button-secondary:hover {
            background: rgba(67, 97, 238, 0.05);
            transform: translateY(-2px);
        }
        
        /* Results */
        .results {
            display: none;
            margin-top: 40px;
            border-top: 1px solid rgba(0,0,0,0.05);
            padding-top: 30px;
            animation: fadeIn 0.5s ease;
        }
        
        .results-title {
            font-size: 1.8rem;
            margin-bottom: 25px;
            color: var(--dark);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .results-title i {
            color: var(--success);
        }
        
        .comparison {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }
        
        @media (min-width: 768px) {
            .comparison {
                flex-direction: row;
            }
        }
        
        .image-box {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }
        
        .image-container {
            width: 100%;
            max-width: 400px;
            height: auto;
            border: 1px solid rgba(0,0,0,0.1);
            border-radius: var(--radius-md);
            overflow: hidden;
            background: rgba(0,0,0,0.02);
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: var(--shadow-sm);
            transition: var(--transition);
        }
        
        .image-container:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-md);
        }
        
        .image-container img {
            max-width: 100%;
            max-height: 300px;
            object-fit: contain;
        }
        
        .image-info {
            text-align: center;
            width: 100%;
        }
        
        .image-info h3 {
            margin-bottom: 5px;
            color: var(--dark);
        }
        
        .image-info p {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        .stats {
            display: flex;
            justify-content: space-between;
            margin-top: 30px;
            padding: 25px;
            background: rgba(67, 97, 238, 0.03);
            border-radius: var(--radius-md);
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .stat-item {
            text-align: center;
            flex: 1;
            min-width: 150px;
        }
        
        .stat-value {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: var(--gray);
        }
        
        .savings {
            color: var(--success) !important;
        }
        
        .actions {
            display: flex;
            gap: 15px;
            margin-top: 30px;
            flex-wrap: wrap;
            justify-content: center;
        }
        
        /* Ad Container */
        .ad-container {
            margin: 40px 0;
            background: white;
            border-radius: var(--radius-md);
            padding: 20px;
            text-align: center;
            min-height: 100px;
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: var(--shadow-sm);
        }
        
        .ad-label {
            font-size: 0.8rem;
            color: var(--gray);
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 10px;
        }
        
        /* Footer */
        footer {
            margin-top: 60px;
            text-align: center;
            color: var(--gray);
            font-size: 0.9rem;
            padding-top: 30px;
            border-top: 1px solid rgba(0,0,0,0.1);
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        
        .footer-links a {
            color: var(--gray);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            color: var(--primary);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 20px;
        }
        
        .social-links a {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(0,0,0,0.05);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--gray);
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }
        
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* Spinner */
        .spinner {
            display: none;
            width: 50px;
            height: 50px;
            margin: 30px auto;
            border: 4px solid rgba(67, 97, 238, 0.1);
            border-radius: 50%;
            border-top: 4px solid var(--primary);
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Toast */
        .toast {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--dark);
            color: white;
            padding: 15px 25px;
            border-radius: var(--radius-sm);
            box-shadow: var(--shadow-lg);
            transform: translateY(100px);
            opacity: 0;
            transition: var(--transition);
            z-index: 1000;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .toast.show {
            transform: translateY(0);
            opacity: 1;
        }
        
        .toast.success {
            background: var(--success);
        }
        
        .toast.error {
            background: var(--danger);
        }
        
        .toast.warning {
            background: var(--warning);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 15px;
            }
            
            nav ul {
                margin-top: 10px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .hero {
                padding: 30px 20px;
            }
            
            .compressor-container {
                padding: 25px;
            }
            
            .upload-area {
                padding: 40px 15px;
            }
            
            .buttons {
                flex-direction: column;
            }
            
            .button {
                width: 100%;
            }
            
            .stats {
                flex-direction: column;
                align-items: center;
            }
            
            .stat-item {
                min-width: 100%;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-content">
            <a href="/" class="logo">
                <div class="logo-icon">
                    <i class="fas fa-compress-alt"></i>
                </div>
                <div class="logo-text">ImageCompressor</div>
            </a>
            <nav>
                <ul>
                    <li><a href="/">Home</a></li>
                    <li><a href="/features">Features</a></li>
                    <li><a href="/how-it-works">How It Works</a></li>
                    <li><a href="/contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <div class="container">
        <!-- Top Ad Banner -->
        <div class="ad-container">
            <div>
                <div class="ad-label">Advertisement</div>
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-2102167174456955"></script>
                <!-- ImageCompressor_Top_Banner -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-2102167174456955"
                     data-ad-slot="YOUR_AD_SLOT_ID"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>
        
        <main class="main-content">
            <div class="hero">
                <h1>Beautiful Image Compression</h1>
                <p class="description">
                    Optimize your images without sacrificing quality. Our advanced compression algorithm reduces file size while maintaining visual perfection.
                </p>
                <div class="features">
                    <div class="feature">
                        <i class="fas fa-bolt"></i>
                        <span>Fast Processing</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-lock"></i>
                        <span>Secure & Private</span>
                    </div>
                    <div class="feature">
                        <i class="fas fa-image"></i>
                        <span>Multiple Formats</span>
                    </div>
                </div>
            </div>
            
            <div class="compressor-container">
                <div class="upload-area" id="upload-area">
                    <div class="upload-icon">
                        <i class="fas fa-cloud-upload-alt"></i>
                    </div>
                    <div class="upload-text">Drag & Drop your image here</div>
                    <div class="upload-subtext">or click to browse files (max 10MB)</div>
                    <input type="file" id="file-input" accept="image/*">
                </div>
                
                <div class="file-preview" id="file-preview">
                    <img id="preview-image" src="" alt="Preview">
                    <div class="file-info" id="file-info"></div>
                </div>
                
                <div class="controls">
                    <div class="control-group">
                        <div class="control-header">
                            <i class="fas fa-sliders-h"></i>
                            <label for="quality-slider">Compression Level</label>
                        </div>
                        <p class="control-description">Adjust the quality to balance between file size and image quality</p>
                        <div class="slider-container">
                            <input type="range" id="quality-slider" min="10" max="100" value="80">
                            <span class="slider-value" id="quality-value">80%</span>
                        </div>
                    </div>
                    
                    <div class="control-group">
                        <div class="control-header">
                            <i class="fas fa-file-image"></i>
                            <label>Output Format</label>
                        </div>
                        <p class="control-description">Choose your preferred output image format</p>
                        <div class="format-options">
                            <div class="format-option selected" data-format="original">
                                <i class="fas fa-file"></i>
                                <span>Original</span>
                            </div>
                            <div class="format-option" data-format="jpeg">
                                <i class="fas fa-file-image"></i>
                                <span>JPEG</span>
                            </div>
                            <div class="format-option" data-format="png">
                                <i class="fas fa-file-image"></i>
                                <span>PNG</span>
                            </div>
                            <div class="format-option" data-format="webp">
                                <i class="fas fa-file-image"></i>
                                <span>WebP</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="buttons">
                        <button id="compress-btn" class="button button-primary" disabled>
                            <i class="fas fa-compress-alt"></i>
                            <span>Compress Image</span>
                        </button>
                        <button id="reset-btn" class="button button-secondary">
                            <i class="fas fa-redo"></i>
                            <span>Reset</span>
                        </button>
                    </div>
                </div>
                
                <div class="spinner" id="spinner"></div>
                
                <div class="results" id="results">
                    <h2 class="results-title">
                        <i class="fas fa-check-circle"></i>
                        Compression Results
                    </h2>
                    
                    <div class="comparison">
                        <div class="image-box">
                            <div class="image-container">
                                <img id="original-image" src="" alt="Original image">
                            </div>
                            <div class="image-info">
                                <h3>Original Image</h3>
                                <p id="original-info">-</p>
                            </div>
                        </div>
                        
                        <div class="image-box">
                            <div class="image-container">
                                <img id="compressed-image" src="" alt="Compressed image">
                            </div>
                            <div class="image-info">
                                <h3>Compressed Image</h3>
                                <p id="compressed-info">-</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="stats">
                        <div class="stat-item">
                            <div class="stat-value savings" id="savings-percent">0%</div>
                            <div class="stat-label">Size Reduction</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-value" id="original-size">0 KB</div>
                            <div class="stat-label">Original Size</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-value" id="compressed-size">0 KB</div>
                            <div class="stat-label">Compressed Size</div>
                        </div>
                    </div>
                    
                    <div class="actions">
                        <button id="download-btn" class="button button-primary">
                            <i class="fas fa-download"></i>
                            <span>Download Compressed Image</span>
                        </button>
                        <button id="new-image-btn" class="button button-secondary">
                            <i class="fas fa-plus"></i>
                            <span>Compress Another Image</span>
                        </button>
                    </div>
                </div>
            </div>
        </main>
        
        <!-- Middle Ad Banner -->
        <div class="ad-container">
            <div>
                <div class="ad-label">Advertisement</div>
                <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-2102167174456955"></script>
                <!-- ImageCompressor_Middle_Banner -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-2102167174456955"
                     data-ad-slot="YOUR_AD_SLOT_ID_2"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>
    </div>
    
    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
            </div>
            <div class="footer-links">
                <a href="/privacy">Privacy Policy</a>
                <a href="/terms">Terms of Service</a>
                <a href="/contact">Contact Us</a>
                <a href="/blog">Blog</a>
            </div>
            <p>&copy; <span id="current-year"></span> ImageCompressorPro. All rights reserved.</p>
        </div>
    </footer>
    
    <div class="toast" id="toast"></div>
    
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('current-year').textContent = new Date().getFullYear();
            
            // DOM elements
            const uploadArea = document.getElementById('upload-area');
            const fileInput = document.getElementById('file-input');
            const filePreview = document.getElementById('file-preview');
            const previewImage = document.getElementById('preview-image');
            const fileInfo = document.getElementById('file-info');
            const qualitySlider = document.getElementById('quality-slider');
            const qualityValue = document.getElementById('quality-value');
            const formatOptions = document.querySelectorAll('.format-option');
            const compressBtn = document.getElementById('compress-btn');
            const resetBtn = document.getElementById('reset-btn');
            const spinner = document.getElementById('spinner');
            const resultsSection = document.getElementById('results');
            const originalImage = document.getElementById('original-image');
            const compressedImage = document.getElementById('compressed-image');
            const originalInfo = document.getElementById('original-info');
            const compressedInfo = document.getElementById('compressed-info');
            const savingsPercent = document.getElementById('savings-percent');
            const originalSize = document.getElementById('original-size');
            const compressedSize = document.getElementById('compressed-size');
            const downloadBtn = document.getElementById('download-btn');
            const newImageBtn = document.getElementById('new-image-btn');
            const toast = document.getElementById('toast');
            
            // Variables
            let selectedFile = null;
            let selectedFormat = 'original';
            let compressedBlob = null;
            
            // Event listeners
            uploadArea.addEventListener('click', () => fileInput.click());
            
            fileInput.addEventListener('change', handleFileSelect);
            
            uploadArea.addEventListener('dragover', (e) => {
                e.preventDefault();
                uploadArea.classList.add('active');
            });
            
            uploadArea.addEventListener('dragleave', () => {
                uploadArea.classList.remove('active');
            });
            
            uploadArea.addEventListener('drop', (e) => {
                e.preventDefault();
                uploadArea.classList.remove('active');
                
                if (e.dataTransfer.files.length) {
                    fileInput.files = e.dataTransfer.files;
                    handleFileSelect({ target: fileInput });
                }
            });
            
            qualitySlider.addEventListener('input', () => {
                qualityValue.textContent = `${qualitySlider.value}%`;
            });
            
            formatOptions.forEach(option => {
                option.addEventListener('click', () => {
                    formatOptions.forEach(opt => opt.classList.remove('selected'));
                    option.classList.add('selected');
                    selectedFormat = option.dataset.format;
                });
            });
            
            compressBtn.addEventListener('click', compressImage);
            resetBtn.addEventListener('click', resetTool);
            downloadBtn.addEventListener('click', downloadCompressedImage);
            newImageBtn.addEventListener('click', resetTool);
            
            // Functions
            function handleFileSelect(event) {
                const file = event.target.files[0];
                
                if (!file) return;
                
                if (!file.type.match('image.*')) {
                    showToast('Please select an image file (JPEG, PNG, etc.)', 'error');
                    return;
                }
                
                if (file.size > 10 * 1024 * 1024) {
                    showToast('Image size should be less than 10MB', 'error');
                    return;
                }
                
                selectedFile = file;
                compressBtn.disabled = false;
                
                // Display preview
                const reader = new FileReader();
                reader.onload = function(e) {
                    previewImage.src = e.target.result;
                    fileInfo.textContent = `${file.name} • ${formatBytes(file.size)} • ${file.type}`;
                    filePreview.style.display = 'block';
                    
                    // Animate the appearance
                    filePreview.style.animation = 'fadeIn 0.5s ease';
                };
                reader.readAsDataURL(file);
                
                // Update upload area text
                uploadArea.querySelector('.upload-text').textContent = 'File selected';
                uploadArea.querySelector('.upload-subtext').textContent = file.name;
            }
            
            function compressImage() {
                if (!selectedFile) return;
                
                // Show loading spinner
                spinner.style.display = 'block';
                compressBtn.disabled = true;
                compressBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> <span>Compressing...</span>';
                
                // Use setTimeout to allow UI to update before compression starts
                setTimeout(() => {
                    const quality = parseInt(qualitySlider.value) / 100;
                    const img = new Image();
                    
                    img.onload = function() {
                        const canvas = document.createElement('canvas');
                        const ctx = canvas.getContext('2d');
                        
                        // Calculate new dimensions if needed (optional)
                        let width = img.width;
                        let height = img.height;
                        
                        // Set canvas dimensions
                        canvas.width = width;
                        canvas.height = height;
                        
                        // Draw image on canvas
                        ctx.drawImage(img, 0, 0, width, height);
                        
                        // Determine output format
                        let mimeType = selectedFile.type;
                        if (selectedFormat !== 'original') {
                            mimeType = `image/${selectedFormat}`;
                            if (selectedFormat === 'jpeg') mimeType = 'image/jpeg';
                        }
                        
                        // Convert to blob with specified quality
                        canvas.toBlob(function(blob) {
                            compressedBlob = blob;
                            
                            // Display compressed image
                            const compressedUrl = URL.createObjectURL(blob);
                            originalImage.src = URL.createObjectURL(selectedFile);
                            compressedImage.src = compressedUrl;
                            
                            originalInfo.textContent = `${formatBytes(selectedFile.size)} • ${selectedFile.type}`;
                            compressedInfo.textContent = `${formatBytes(blob.size)} • ${mimeType}`;
                            
                            // Calculate and display stats
                            const originalSizeBytes = selectedFile.size;
                            const compressedSizeBytes = blob.size;
                            const savings = ((originalSizeBytes - compressedSizeBytes) / originalSizeBytes) * 100;
                            
                            originalSize.textContent = formatBytes(originalSizeBytes);
                            compressedSize.textContent = formatBytes(compressedSizeBytes);
                            savingsPercent.textContent = `${Math.round(savings)}%`;
                            
                            // Show results
                            resultsSection.style.display = 'block';
                            spinner.style.display = 'none';
                            compressBtn.innerHTML = '<i class="fas fa-compress-alt"></i> <span>Compress Image</span>';
                            
                            // Scroll to results
                            setTimeout(() => {
                                resultsSection.scrollIntoView({ behavior: 'smooth' });
                            }, 100);
                            
                            // Show success toast
                            showToast('Image compressed successfully!', 'success');
                            
                        }, mimeType, quality);
                    };
                    
                    img.src = URL.createObjectURL(selectedFile);
                }, 100);
            }
            
            function downloadCompressedImage() {
                if (!compressedBlob) return;
                
                const url = URL.createObjectURL(compressedBlob);
                const a = document.createElement('a');
                a.href = url;
                
                // Set filename
                const originalName = selectedFile.name.split('.')[0];
                let extension = selectedFile.type.split('/')[1];
                if (selectedFormat !== 'original') {
                    extension = selectedFormat;
                    if (selectedFormat === 'jpeg') extension = 'jpg';
                }
                
                a.download = `${originalName}-compressed.${extension}`;
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                URL.revokeObjectURL(url);
                
