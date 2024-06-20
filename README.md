## Flask Application Design

### HTML Files

**index.html**
- Main page of the application.
- Presents a form for the user to input a company name and announcement date.

**results.html**
- Displays the results of the analysis, including the impact on the share price and relevant news articles.

### Routes

**@app.route('/')**
- Renders the `index.html` file, displaying the main page.

**@app.route('/results')**
- Receives the input from the form and calls the analysis function.
- Renders the `results.html` file, displaying the results.

**@app.route('/analysis')**
- Behind-the-scenes function to perform the analysis.
- Analyzes the impact of the announcement on the share price and retrieves news articles.
- Returns the results in a JSON format.