
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SpendWise Dashboard</title>

    <style>
        /* ROOT VARIABLES */
        :root {
            --brand-color: #2563eb;
            --accent-color: #14b8a6;
            --background-color: #f1f5f9;
            --surface-color: #ffffff;
            --primary-text: #1e293b;
            --secondary-text: #64748b;
            --border-color: #e2e8f0;
        }

        /* GENERAL STYLING */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: var(--background-color);
            color: var(--primary-text);
        }

        a {
            text-decoration: none;
        }

        /* MAIN GRID LAYOUT */
        .dashboard {
            display: grid;
            grid-template-columns: 250px 1fr;
            min-height: 100vh;
        }

        /* SIDEBAR */
        .sidebar {
            background: var(--surface-color);
            padding: 30px 20px;
            display: flex;
            flex-direction: column;
            border-right: 1px solid var(--border-color);
        }

        .logo {
            color: var(--brand-color);
            margin-bottom: 40px;
            font-size: 26px;
        }

        .navigation {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .navigation a {
            color: var(--secondary-text);
            padding: 14px;
            border-radius: 8px;
            transition: background 200ms ease;
        }

        .navigation a:hover,
        .navigation a:focus-visible,
        .navigation .active {
            background: var(--brand-color);
            color: white;
        }

        .sidebar-footer {
            margin-top: auto;
            padding-top: 30px;
            color: var(--secondary-text);
        }

        .sidebar-footer p {
            font-weight: bold;
            margin-bottom: 8px;
        }

        /* MAIN CONTENT */
        .main-content {
            padding: 30px;
            min-width: 0;
        }

        /* HEADER FLEXBOX */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
        }

        .header h1 {
            margin-bottom: 8px;
        }

        .header p {
            color: var(--secondary-text);
        }

        .profile {
            display: flex;
            align-items: center;
            gap: 15px;
            color: var(--secondary-text);
        }

        .avatar {
            background: var(--brand-color);
            color: white;
            width: 42px;
            height: 42px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: bold;
        }

        /* OVERVIEW CARDS */
        .overview {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-bottom: 40px;
        }

        .overview-card {
            background: var(--surface-color);
            padding: 24px;
            border-radius: 12px;
            border: 1px solid var(--border-color);
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .overview-card p,
        .overview-card small {
            color: var(--secondary-text);
        }

        .overview-card h2 {
            color: var(--brand-color);
            font-size: 25px;
        }

        /* CATEGORY SECTION */
        .section-heading {
            margin-bottom: 20px;
        }

        .section-heading h2 {
            margin-bottom: 8px;
        }

        .section-heading p {
            color: var(--secondary-text);
        }

        /* CATEGORY GRID */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 20px;
        }

        /* CATEGORY CARDS */
        .category-card {
            background: var(--surface-color);
            border: 1px solid var(--border-color);
            padding: 24px;
            border-radius: 12px;

            display: flex;
            flex-direction: column;
            gap: 14px;

            transition: transform 200ms ease,
                        box-shadow 200ms ease;
        }

        /* HOVER AND KEYBOARD FOCUS */
        .category-card:hover,
        .category-card:focus-visible {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.10);
            outline: 2px solid var(--brand-color);
            outline-offset: 2px;
        }

        .card-top {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .icon {
            font-size: 28px;
        }

        .status {
            background: var(--background-color);
            color: var(--accent-color);
            padding: 6px 10px;
            border-radius: 20px;
            font-size: 12px;
        }

        .category-card h3 {
            font-size: 18px;
        }

        .category-card h2 {
            color: var(--brand-color);
            font-size: 25px;
        }

        .category-card p {
            color: var(--secondary-text);
            font-size: 14px;
        }

        /* FOOTER */
        .footer {
            margin-top: 40px;
            padding: 20px 0;
            border-top: 1px solid var(--border-color);
            color: var(--secondary-text);
            text-align: center;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 767px) {
            .dashboard {
                grid-template-columns: 1fr;
            }

            .sidebar {
                padding: 20px;
            }

            .logo {
                margin-bottom: 20px;
            }

            .navigation {
                flex-direction: row;
                flex-wrap: wrap;
            }

            .navigation a {
                padding: 10px;
            }

            .sidebar-footer {
                margin-top: 20px;
            }

            .main-content {
                padding: 20px;
            }

            .header {
                flex-direction: column;
                align-items: flex-start;
            }

            .overview {
                grid-template-columns: 1fr;
            }

            .card-grid {
                grid-template-columns: 1fr;
            }

            .profile {
                margin-top: 10px;
            }
        }

        /* DARK THEME */
        @media (prefers-color-scheme: dark) {
            :root {
                --brand-color: #60a5fa;
                --accent-color: #2dd4bf;
                --background-color: #0f172a;
                --surface-color: #1e293b;
                --primary-text: #f8fafc;
                --secondary-text: #cbd5e1;
                --border-color: #334155;
            }
        }

    </style>
</head>

<body>

    <div class="dashboard">

        <!-- SIDEBAR -->
        <aside class="sidebar">

            <h2 class="logo">SpendWise</h2>

            <nav class="navigation">
                <a href="#" class="active">Dashboard</a>
                <a href="#">My Transactions</a>
                <a href="#">Budgets</a>
                <a href="#">Savings</a>
                <a href="#">Reports</a>
                <a href="#">Settings</a>
            </nav>

            <div class="sidebar-footer">
                <p>Personal Finance</p>
                <small>Manage your money wisely.</small>
            </div>

        </aside>

        <!-- MAIN CONTENT -->
        <main class="main-content">

            <!-- HEADER -->
            <header class="header">

                <div>
                    <h1>Dashboard</h1>
                    <p>Welcome back! Here's your financial overview.</p>
                </div>

                <div class="profile">
                    <span>November 2026</span>
                    <div class="avatar">DS</div>
                </div>

            </header>

            <!-- FINANCIAL OVERVIEW -->
            <section class="overview">

                <div class="overview-card">
                    <p>Total Balance</p>
                    <h2>$8,450.00</h2>
                    <small>Available balance</small>
                </div>

                <div class="overview-card">
                    <p>Total Income</p>
                    <h2>$4,800.00</h2>
                    <small>Monthly income</small>
                </div>

                <div class="overview-card">
                    <p>Total Expenses</p>
                    <h2>$2,150.00</h2>
                    <small>Monthly expenses</small>
                </div>

            </section>

            <!-- EXPENSE CATEGORIES -->
            <section class="categories">

                <div class="section-heading">
                    <h2>Expense Categories</h2>
                    <p>November spending overview</p>
                </div>

                <div class="card-grid">

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">🍔</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Food</h3>
                        <h2>$450.00</h2>
                        <p>Groceries and restaurants</p>
                    </article>

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">🚗</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Transport</h3>
                        <h2>$180.00</h2>
                        <p>Travel and fuel expenses</p>
                    </article>

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">🏠</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Rent</h3>
                        <h2>$800.00</h2>
                        <p>Monthly accommodation</p>
                    </article>

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">🎬</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Entertainment</h3>
                        <h2>$120.00</h2>
                        <p>Movies and recreation</p>
                    </article>

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">💰</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Savings</h3>
                        <h2>$400.00</h2>
                        <p>Future financial goals</p>
                    </article>

                    <article class="category-card" tabindex="0">
                        <div class="card-top">
                            <span class="icon">💡</span>
                            <span class="status">Monthly</span>
                        </div>
                        <h3>Utilities</h3>
                        <h2>$200.00</h2>
                        <p>Electricity, water and internet</p>
                    </article>

                </div>
            </section>

            <!-- FOOTER -->
            <footer class="footer">
                <p>© 2026 SpendWise. Manage your money wisely.</p>
            </footer>

        </main>

    </div>

</body>
</html>
