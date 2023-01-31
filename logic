def droop_control(measured_frequency, reference_frequency, kp, ki):
    # Initialize variables to keep track of the error and integral of the error
    error = reference_frequency - measured_frequency
    integral = 0
    
    # Integrate the error over time to calculate the integral
    integral += error * dt
    
    # Calculate the control signal using the proportional and integral gains
    control_signal = kp * error + ki * integral
    
    # Update the inverter output based on the control signal
    inverter_output = inverter_output + control_signal
    
    # Return the updated inverter output
    return inverter_output
