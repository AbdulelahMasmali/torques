# torques

<img width="363" height="424" alt="image" src="https://github.com/user-attachments/assets/8c6ba917-0fc0-4c9f-9857-d7960e3c2d63" />

the tasks is 

Task 1: Calculate the required torque for each motor in the robotic arm to carry a weight of 1 kg, and search for suitable servo motors for each joint.

task 2: Can the same motors selected in the previous task lift a weight of 2 kg instead of 1 kg by adding some gears? What challenges will the robotic arm face, and what are the alternatives to address these challenges?

------

task 1

mass m = 1 kg

gravity g = 9.8 m/s²

Link lengths
L1 = 0.15m 
L2 = 0.10m 
L3 = 0.04m

torque formula τ = r ⋅ F where F = m ⋅ g and r is the distance from the joint to the weight

joint 3 end: τ3 = F ⋅ L3 = (1 ⋅ 9.8) ⋅ 0.04 = 0.392 Nm

joint 2 middle: τ2 = F ⋅ (L2 + L3) = 9.8 ⋅ 0.14 = 1.372 Nm

joint 1 base: τ1 = F ⋅ (L1 + L2 + L3) = 9.8 ⋅ 0.29 = 2.842 Nm

convert Nm to kg·cm (1 Nm ≈ 10.2 kg·cm)

τ1 ≈ 29 kg·cm τ2 ≈ 14 kg·cm τ3 ≈ 4 kg·cm

suitable servos

Joint 1 MG995 
https://bit.ly/4oIxqSX

Joint 2 MG996R 
https://bit.ly/43ouz9j

Joint 3 MG90S 
https://bit.ly/4868oHo

---------------------------------------------------------------------------------------------------------------------

task 2 

Yes, you can increase the load to 2 kg with the same servos by adding gear reduction but there are trade offs

Torque requirement for 2 kg

Torque doubles because the weight doubles

Joint 1   2 × 29 ≈ 58 kg·cm

Joint 2   2 × 14 ≈ 28 kg·cm

Joint 3   2 × 4 ≈ 8 kg·cm

Using gear reduction increases the torque but it has negatives for example reduced speed, more friction, and backlash.

For better solutions Use higher torque servos
