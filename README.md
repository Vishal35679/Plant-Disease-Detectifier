# Plant-Disease-Detectifier

**PlantCPU.ipynb**
CUDA was throwing error so i started working with cpu and it takes very long time to execute 
![Screenshot 2023-05-09 003127](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/866669fa-e19e-4d98-b9eb-f9a57aba7b52)
![Screenshot 2023-05-09 150810](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/0142a900-2e2f-407c-959d-6c45f387f89f)
I knew that cpu is not gonna complete the task so i have to use GPU
Then i installed CUDA but still got the error that torch is not compiled with CUDA 
then i thought of using the CUDA and CUdnn for the pytorch installed and completed installation process Finally it was working
![Screenshot 2023-05-13 093407](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/e2f8a8b7-427f-46a8-8053-516912316db9)
the first step was executed with so less time compared to cpu process i got hopes
![Screenshot 2023-05-13 105822](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/d9caddae-0d29-4c8c-b77b-40d5fb29dade)
and then this happened
![Screenshot 2023-05-13 110548](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/d431cc71-26cf-497d-9e1d-2d744c028f1e)
i was getting same error after running multiple time 
then i started looking how to tackle with this problem 
i came across the idea to reduce the batch size
i reduced the size to 28 from 32 then 24, 20, 16 and finally 8
finally it started running even though it used almost 3.9gb out of 4gb still it executed after long time
![Screenshot 2023-05-13 171106](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/7720dfac-ea11-46f1-bf70-867150d1f1ea)
after waiting for some more it finally completed
![Screenshot 2023-05-13 185131](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/52ba89dd-fc99-4f1f-829f-7d02cca0bb8d)
finally it was executed with accuracy of 97.52
![Screenshot 2023-05-13 185204](https://github.com/Vishal35679/Plant-Disease-Detectifier/assets/104795331/a376c8a0-f82f-47c2-9457-f1fa24e6daed)
but we need accuracy of more than 99.2 
