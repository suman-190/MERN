# MERN
# MERN

'''

import { useState } from 'react'
import { Button } from './components/button/Button'
import { FaRegTrashAlt } from "react-icons/fa";


function App() {
  
  const [name, setName] = useState('')
  const [data, setData] = useState([])
  const handleChange = (e) => {
  
   setName(e.target.value)
    
  }


const fetchdata = async () => {
  const res= await fetch('https://jsonplaceholder.typicode.com/todos/10')
   const resData =  await res.json()
   setData(resData)

   
     
}


fetchdata()

  return (  
    <div>
     

     <input type="text" placeholder="Enter your name" onChange={handleChange} />
     <button>ADD</button>
     <h1>Todo:{name}</h1>
     <div>
        <div>
          {}
        </div>
     </div>
    
   
    </div>
      
  )
}

export default App

'''