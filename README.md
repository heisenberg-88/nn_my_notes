# nn_my_notes
personal code snippets notes


# Pytorch CUDA usage /checks

    import torch 
    torch.cuda.is_available()
    
   TRUE if CUDA is available as device = CUDA:0
   otherwise FALSE
   
   
    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
    print(device)
    
   Prints CUDA:0 if GPU is available with CUDA
   
    
   To transfer nn or any tensors to GPU with CUDA,
    
   if Tenssor is X,
      
      x.to(device)
   this will transfer the tensor to CUDA device
   
   if neuralNet is defined by net ,
    
     net.to(device)
    
 
 
