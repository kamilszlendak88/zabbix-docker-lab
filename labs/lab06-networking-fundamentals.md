# LAB 06 – Networking Fundamentals for SRE

## Goal
Understand and validate the full network connection flow:
DNS → IP → Port → TCP → HTTP.

## DNS resolution
Verified hostname resolution using getent.
This confirmed correct DNS configuration on the system.

## TCP and HTTP connectivity
Tested HTTP connectivity using curl.
Confirmed successful TCP connection and HTTP response.

## Failure scenario
Attempted to connect to a non-listening port.
Observed connection failure, demonstrating port-level issues.

## Localhost testing
Compared connections using localhost and 127.0.0.1.
Validated local networking behavior.

## Result
Successfully practiced systematic network troubleshooting
by isolating issues at each layer of the connection process.

## Localhost testing
Connection attempts to localhost (127.0.0.1) on port 80 failed
because no local HTTP service was running.
This demonstrated that localhost connectivity depends on
locally running services, not external network access.
