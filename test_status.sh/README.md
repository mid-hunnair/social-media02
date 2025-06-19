#!/bin/bash
echo "🔍 Running basic CI test..."

if [ -f "facebook/README.md" ]; then
    echo "✅ Facebook README exists - Test Passed!"
    exit 0
else
    echo "❌ Facebook README missing - Test Failed!"
    exit 1
fi

