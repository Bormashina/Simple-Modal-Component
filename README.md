# Simple-Modal-Component
React.js Code for a Simple Modal Component
import React, { useState } from 'react';

function Modal() {
    const [isOpen, setIsOpen] = useState(false);

    return (
        <div>
            <button onClick={() => setIsOpen(true)}>Open Modal</button>
            {isOpen && (
                <div>
                    <p>Modal Content</p>
                    <button onClick={() => setIsOpen(false)}>Close Modal</button>
                </div>
            )}
        </div>
    );
}

export default Modal;
