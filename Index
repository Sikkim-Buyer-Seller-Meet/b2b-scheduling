import React, { useState } from "react";

const SimpleForm = () => {
    const [formData, setFormData] = useState({
        name: "",
        number: "",
        company: "",
        email: ""
    });

    const handleChange = (e) => {
        setFormData({ ...formData, [e.target.name]: e.target.value });
    };

    const handleSubmit = (e) => {
        e.preventDefault();
        console.log("Form submitted:", formData);
        alert("Form submitted successfully!");
    };

    return (
        <div className="flex justify-center items-center h-screen bg-gray-100">
            <div className="bg-white p-6 rounded-lg shadow-lg w-96">
                <h2 className="text-xl font-bold mb-4">Basic Information</h2>
                <form onSubmit={handleSubmit}>
                    <label className="block">Name:</label>
                    <input type="text" name="name" value={formData.name} onChange={handleChange} className="w-full p-2 border rounded" required />
                    
                    <label className="block mt-2">Number:</label>
                    <input type="tel" name="number" value={formData.number} onChange={handleChange} className="w-full p-2 border rounded" required />
                    
                    <label className="block mt-2">Company:</label>
                    <input type="text" name="company" value={formData.company} onChange={handleChange} className="w-full p-2 border rounded" required />
                    
                    <label className="block mt-2">Email:</label>
                    <input type="email" name="email" value={formData.email} onChange={handleChange} className="w-full p-2 border rounded" required />
                    
                    <button type="submit" className="w-full mt-4 p-2 bg-blue-600 text-white rounded hover:bg-blue-800">Submit</button>
                </form>
            </div>
        </div>
    );
};

export default SimpleForm;
