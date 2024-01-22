# BlogApp
Overview
This repository encapsulates my successful completion of the second technical round's MERN stack task. From MongoDB to Express.js, React.js, and Node.js, this project demonstrates my proficiency in building robust full-stack applications.
<br>
<br>
Highlights
Tech Stack Mastery: Leveraged MongoDB for the database, utilized Express.js for server-side logic, implemented a dynamic front end with React.js, and ensured smooth integration using Node.js.

<br>
Code Quality: Emphasized clean and modular code practices, making the codebase easy to understand, maintain, and scale.
<br>
<br>
# Kindly ensure the seamless execution of the project by installing the necessary packages using 'npm install' before running !!

npm install react react-dom redux react-redux @reduxjs/toolkit axios express mongoose cors body-parser mongodb <br>
npm install @mui/material @emotion/react @emotion/styled  # Or install Bootstrap for styling
 crate server.js
 <br>
 <br>
 <br>
// Import necessary modules
Connect to MongoDB
mongoose.connect('mongodb://localhost:27017/blog', { useNewUrlParser: true })
    .then(() => console.log('MongoDB connected'))
    .catch(err => console.error(err));
<br>
<br>
// Define Mongoose schema for articles
const articleSchema = new mongoose.Schema({
    title: String,
    description: String,
    category: String,
    createdAt: Date,
    updatedAt: Date
});
<br>
<br>
// Create Mongoose model
const Article = mongoose.model('Article', articleSchema);
<br>
<br>
// Create Express app
const app = express();
<br>
<br>
// Middlewares
app.use(cors());
app.use(bodyParser.json());
<br>
<br>
// API routes for CRUD operations
// ...
<br>
<br>
// Start the server
app.listen(3000, () => console.log('Server started on port 3000'));
<br>
<br>

# Thank You !
