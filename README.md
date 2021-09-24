# student-mark-sheet
showing student marksheet
const end= require('express');
const app=end();

app.use(end.json());




const arr=[
    {id:1,student1:[{subject1:100},
    
        {subject2:98},{subject:76},{subject4:80},{subject5:90},
    
    
    ]},
    {id:2,student2:[{subject1:90},
    
        {subject2:80},{subject3:40},{subject4:90},{subject5:70},
    
    
    ]},
    {id:3,student3:[{subject1:50},
    
        {subject2:80},{subject3:50},{subject4:90},{subject5:50},
    
    
    ]},
    {id:4,student4:[{subject1:50},
    
        {subject2:50},{subject3:50},{subject4:50},{subject5:50}
    
    ]}
]


app.get('/',(req,res)=>{
    res.send(arr)
})

app.get('/api/post',(req,res)=>{

    res.send(arr);

})


app.post('/api/post',(req,res)=>{

const hod={
    id:students.length+1,
    arr:req.body.subject,
};

arr.push(hod);
res.send(hod);

})

app.put('/api/post/:id',(req,res)=>{

 const update= arr.find(up=>up.id===parseInt(req.params.id))


 arr.subject=req.body.subject;

//  subject=req.body.subject
//  student:req.body.subject,
res.send(update)
})


app.delete('/api/post/:id',(req,res)=>{
  const value= arr.find(sai=>sai.id===parseInt(req.params.id));
dy
  const index=arr.indexOf(value);
  arr.splice(index,1)
  res.send(value)


})


app.listen(3000,()=>console.log('listing port is 3000'));



console.log(arr);

var a = document.getElementsByTagName('h1');

body.append(a);
