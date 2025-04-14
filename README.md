<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Heim - Technology Solutions</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2563eb;
            --dark: #1e293b;
            --light: #f8fafc;
            --accent: #f59e0b;
            --gray: #94a3b8;
        }
        
* {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }
        
  .techheim-header {
            background: white;
            padding: 1rem 5%;
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
  .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1400px;
            margin: 0 auto;
            gap: 2rem;
        }
        
  .branding {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
  .logo {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--dark);
            white-space: nowrap;
        }
        
   .search-container {
            flex: 1;
            max-width: 600px;
            position: relative;
        }
        
  .search-bar {
            width: 100%;
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            border: 1px solid var(--gray);
            font-size: 1rem;
            padding-right: 50px;
            transition: all 0.3s;
        }
        
   .search-bar:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.2);
        }
        
   .search-icon {
            position: absolute;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
            color: var(--gray);
        }
        
   .header-actions {
            display: flex;
            gap: 1.5rem;
            align-items: center;
        }
        
   .action-btn {
            display: flex;
            flex-direction: column;
            align-items: center;
            color: var(--dark);
            text-decoration: none;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
  .action-btn i {
            font-size: 1.3rem;
            margin-bottom: 5px;
        }
        
  .action-btn:hover {
            color: var(--primary);
        }
        
  .cart-count {
            background: var(--accent);
            color: white;
            border-radius: 50%;
            width: 18px;
            height: 18px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.7rem;
            position: absolute;
            top: -5px;
            right: -5px;
        }
        
        /* رسپانسیو */
  @media (max-width: 768px) {
            .header-container {
                flex-wrap: wrap;
            }
            
   .search-container {
                order: 3;
                width: 100%;
                margin-top: 1rem;
            }
            
   .branding {
                flex: 1;
            }
        }
    </style>
</head>
<body>
    <header class="techheim-header">
        <div class="header-container">
            <div class="branding">
                <div class="logo">Tech Heim</div>
            </div>
            
   <div class="search-container">
                <input type="text" class="search-bar" placeholder="What can we help you find?">
                <i class="fas fa-search search-icon"></i>
            </div>
            
   <div class="header-actions">
                <a href="#" class="action-btn">
                <i class="fas fa-user"></i>
                    <span>Login</span>
                </a>
                <a href="#" class="action-btn" style="position: relative;">
                    <i class="fas fa-shopping-cart"></i>
                    <span>Cart</span>
                    <span class="cart-count">3</span>
                </a>
            </div>
        </div>
    </header>
</body>
</html>
