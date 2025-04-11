# Motor-codes
RPM values 
 if (current_time - prev_time >= 100) {  // update every 100 ms
        speed = (encoder_count - prev_encoder_count) * 600.0 / 
                (ticks_per_rev * (current_time - prev_time));
        prev_encoder_count = encoder_count;
        prev_time = current_time;
        Serial.println(speed);
    }
