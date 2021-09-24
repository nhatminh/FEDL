# FEDL over Wireless Networks

This repository is a simulation code for the paper

Canh Dinh, Nguyen H. Tran, Minh N. H. Nguyen, Choong Seon Hong, Wei Bao, Albert Y. Zomaya, Vincent Gramoli
"Federated Learning over Wireless Networks: Convergence Analysis and Resource Allocation".
https://arxiv.org/abs/1910.13067

Please run the code in `julia` folder

# FEDL for multiple services
Minh N. H. Nguyen, Nguyen H. Tran, Yan Kyaw Tun, Zhu Han, Choong Seon Hong 
"Toward Multiple Federated Learning Services Resource Sharing in Mobile Edge Networks," 
https://arxiv.org/abs/2011.12469

We use Julia version 1.0.
Please run the code in `multi-services` folder

All of Figures will be generated in `figs` folder.

Main.jl will includes 5 files
- "Setting.jl"
- "TrafficGen.jl"
- "Solving1.jl"
- "Utils.jl" 
- "Plots_Figs.jl"/"Plots_Figs1.jl"

```
Several Setting config parameters as 
if(NUMERICAL_RS)
    # Result for Section V: NUMERICAL RESULTS
    include("Plots_Figs1.jl")
else
    # Result for Section IV: Closed-Form solution
    include("Plots_Figs.jl")
end


READ_RESULT = true		# Read results from result files
NUMERICAL_RS = true     # Result for Section V: NUMERICAL RESULTS in the paper (50 devs)
# NUMERICAL_RS = false  # Result for Section IV: Closed-Form solution in the paper (5 devs)
```

We apply the Federated Learning code from
https://github.com/shaoxiongji/federated-learning
