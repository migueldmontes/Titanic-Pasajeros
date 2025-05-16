import React, { useState } from 'react';
import { Button } from '@/components/ui/button';

const TitanicAndZooApp = () => {
    const [zoo, setZoo] = useState(['León', 'Tigre', 'Elefante', 'Cebra', 'Jirafa']);
    const [passengers, setPassengers] = useState([
        'John', 'Mary', 'Alice', 'Bob', 'Charlie', 'Daisy', 'Edward', 'Fiona', 'George', 'Hannah', 'Ian', 'Jane'
    ]);

    const handleZooUpdates = () => {
        const updatedZoo = [...zoo, 'Panda', 'Koala'];
        updatedZoo.pop();  // Remove the last animal
        updatedZoo[2] = 'Gorila';  // Replace third animal
        setZoo(updatedZoo);
    };

    const handlePassengerUpdates = () => {
        const updatedPassengers = [...passengers];
        updatedPassengers.splice(-2, 2, 'Samuel', 'Olivia');  // Replace last two
        updatedPassengers[1] = 'Lucas';  // Replace second passenger
        setPassengers(updatedPassengers);
    };

    return (
        <div className="p-6 bg-gray-50 min-h-screen">
            <h1 className="text-3xl font-bold mb-6">Inventario del Zoo</h1>
            <p>Animales en el zoo: {zoo.join(', ')}</p>
            <p>Total de animales: {zoo.length}</p>
            <Button onClick={handleZooUpdates} className="my-4">Actualizar Zoo</Button>
            <ul className="list-disc pl-6">
                {zoo.map((animal, index) => (
                    <li key={index}>{animal}</li>
                ))}
            </ul>

            <h1 className="text-3xl font-bold mt-10 mb-6">Lista de Pasajeros del Titanic</h1>
            <ul className="list-disc pl-6">
                {passengers.map((passenger, index) => (
                    <li key={index}>{passenger}</li>
                ))}
            </ul>
            <Button onClick={handlePassengerUpdates} className="my-4">Actualizar Lista de Pasajeros</Button>
        </div>
    );
};

export default TitanicAndZooApp;
